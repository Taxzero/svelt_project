<script>
    let username = "";
    let password = "";
  
    async function handleSubmit() {
      const response = await fetch('https://random-data-api.com/api/v2/users?size=2&is_xml=true');
      const xmlText = await response.text();
      const parser = new DOMParser();
      const xml = parser.parseFromString(xmlText, "application/xml");
      const userNodes = xml.getElementsByTagName("user");
  
      for (let i = 0; i < userNodes.length; i++) {
        const userNode = userNodes[i];
        const id = userNode.querySelector("username").textContent;
        const pw = userNode.querySelector("password").textContent;
  
        if (id === username && pw === password) {
          window.location.href = "C:/svelt/login/src/routes/+2page.svelte";
          return;
        }
      }
  
      alert("Username and password do not match.");
    }
  </script>





<div class ="main-box">
    
    <div class ="box1">
    <br>
    <br>
    <br>
    <h2>Welcom to our Systems</h2>
    <br>
    <h3>Notice</h3>
    <div>
        <!--notice 내용 불러오기-->
    </div>
    <br>
    <a href="#" class="knowmore-button">Know more</a>
    </div>

    <div class = "box2">
        <br>
        <br>
        <br>
        <br>
        <img src="https://www.jejusunresort.com/images/logo.png" alt="logo" width="40%">
        <br>
        <br>
        <br>
        <br>
        <div>
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" bind:value={username}>
    </div>
    <br />
    <div>
      <label for="pass">Password</label>
      <input type="password" id="password" name="password" bind:value={password}>
    </div>
        </div>
        <br>
        <br>
        <br>
        <button on:click={handleSubmit}>Submit</button>
    </div>

<style>
    

h2 {
    color: white;
    font-family: 'Open Sans', sans-serif;
    font-size: 1.5em;
    text-align: center;
}

h3 {
    color: white;
    font-family: 'Open Sans', sans-serif;
    font-size: 1em;
    text-align: left;
    margin-left: 40px;
}


input {
  border: 0;
  outline: 0;
  background: transparent;
  border-bottom: 1px solid black;
}

.main-box {
    width: 720px;
    height: 500px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: white;
    box-shadow: 5px 5px 5px 5px gray;
    border-radius: 15px;
}

.box1 {
    width: 360px;
    height: 500px;
    background: linear-gradient(to bottom right, #EC9F05, #FF4E00);
    border-radius: 15px;
}

.box2 {
    width: 360px;
    height: 500px;
    border-radius: 15px;
    text-align: center;
}


.knowmore-button {
    align-items: center;
    display: inline-block;
    padding: 5px 5px;
    border: 2px solid white;
    border-radius: 5px;
    color: white;
    text-align: center; 
    font-family: 'Open Sans', sans-serif;
    font-size: 0.8em;
    margin-left: 40px;
}
.knowmore-button:hover {
    background-color: white;
    color:grey;
}

</style>