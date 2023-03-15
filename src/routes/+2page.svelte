
<div class ="main-box">
    
    <div class ="box1">
        <h2>
            Customer Point
        </h2>
        <div>
            <input type="text" id="username" name="username">
        </div>
        <h3>
            현재 포인트
        </h3>
        <div class ="Pbox">
            <!--고객 포인트 현황-->
        </div>
    </div>

    <div class = "box2">
        <div class="flex-2 flex1">
            <h4>고객 포인트 차감</h4>
            <div class="flex">
                <div class="flex2"><!--좌측-->
                    <h5>객실</h5>
                    <h5>카페 라운지</h5>
                    <h5>로터스</h5>
                    <h5>하우스 오브 바베큐</h5>
                    <h5>가든뷔페</h5>
                    <h5>룸서비스</h5>
                    <h5>부대시설</h5>
                </div>
                <div class="flex3"><!--우측-->
                    <input type="text" id="username" name="username">
                    <br>
                    <input type="text" id="username" name="username">
                    <br>
                    <input type="text" id="username" name="username">
                    <br>
                    <input type="text" id="username" name="username">
                    <br>
                    <input type="text" id="username" name="username">
                    <br>
                    <input type="text" id="username" name="username">
                    <br>
                    <input type="text" id="username" name="username">
                </div>
            </div>
            <a href="#" class="savebutton">save</a>
        </div>
    </div>

</div>

<style>
    

h2 {
    color: white;
    font-family: 'Open Sans', sans-serif;
    font-size: 1.5em;
    text-align: center;
    padding-top: 20%;
    padding-bottom: 20%;
}

h3 {
    color: white;
    font-family: 'Open Sans', sans-serif;
    font-size: 1em;
    text-align: center;
    padding-top: 10%;
}

h4 {
    color: grey;
    font-family: 'Open Sans', sans-serif;
    font-size: 1.5em;
    text-align: center;
    padding-top: 8%;
}

h5 {
    color: grey;
    font-family: 'Open Sans', sans-serif;
    font-size: 1em;
    text-align: center;
}

input {
  border: 0;
  outline: 0;
  background: transparent;
  border-bottom: 1px solid grey;
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
    width: 300px;
    height: 500px;
    background: linear-gradient(to bottom right, #EC9F05, #FF4E00);
    border-radius: 15px;
    text-align: center;
}

.box2 {
    width: 420px;
    height: 500px;
    border-radius: 15px;
    text-align: center;
}

.Pbox{
    width: 180px;
    height: 20px;
    margin-left: 60px;
    background-color: white;
}

.flex{
    display:flex;
    flex-direction: row
}

.flex-2{
    display:flex;
    flex-direction: column;}

.flex1{
    justify-content: center;
    align-content: center;
    align-items: center;
}

.flex2{
    justify-content: felx-start;
    align-content: center;
    align-items: center;
}

.flex3{
    justify-content: flex-end;
    align-content: center;
    align-items: center;
}

.savebutton {
    align-items: center;
    display: inline-block;
    padding: 5px 5px;
    border: 2px solid gray;
    border-radius: 5px;
    color: gray;
    text-align: center; 
    font-family: 'Open Sans', sans-serif;
    font-size: 0.8em;
    margin-left: 40px;
}
.savebutton:hover {
    background-color: white;
    color:grey;
}

</style>