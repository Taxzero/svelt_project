
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
            <input type="text" id="username" name="username">
        </div>
        <br>
        <div>
            <label for="pass">Password</label>
            <input type="password" id="pass" name="password"
                   minlength="8" required>
        </div>
        <br>
        <br>
        <br>
        <input type="submit" value="Sign in">
    </div>

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

h4 {
    color: white;
    font-family: 'Open Sans', sans-serif;
    font-size: 0.8em;
    text-align: left;
    margin-left: 40px;
    margin-right: 40px;
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
    froat: left;
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