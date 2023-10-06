<script>
    let toggleprog = false;
    let togglefront = false;
    let toggleback = false;
    let toggledata = false;
    let toggletest = false;
    let togglemanage = false;
    function proSkills(){
        toggleprog = true;
        togglefront = false;
        toggleback = false;
        toggledata = false;
        toggletest = false;
        togglemanage = false;
    }
    function frontSkills(){
        toggleprog = false;
        togglefront = true;
        toggleback = false;
        toggledata = false;
        toggletest = false;
        togglemanage = false;
    }
    function backSkills(){
        toggleprog = false;
        togglefront = false;
        toggleback = true;
        toggledata = false;
        toggletest = false;
        togglemanage = false;
    }
    function dataSkills(){
        toggleprog = false;
        togglefront = false;
        toggleback = false;
        toggledata = true;
        toggletest = false;
        togglemanage = false;
    }
    function testSkills(){
        toggleprog = false;
        togglefront = false;
        toggleback = false;
        toggledata = false;
        toggletest = true;
        togglemanage = false;
    }
    function manageSkills(){
        toggleprog = false;
        togglefront = false;
        toggleback = false;
        toggledata = false;
        toggletest = false;
        togglemanage = true;
    }
</script>

<body>
<div class="btns">
    <button on:click={proSkills}><strong>Programming Skills</strong></button><br><br>
    <button on:click={frontSkills}><strong>Frontend Skills</strong></button><br><br>
    <button on:click={backSkills}><strong>Backend Skills </strong></button><br><br>
    <button on:click={dataSkills}><strong> Database Management</strong></button><br><br>
    <button on:click={testSkills}><strong>Testing Skills </strong></button><br><br>
    <button on:click={manageSkills}><strong>Project Management Tools </strong></button>

</div>
{#if toggleprog}
<div class="card-programming">
    <div>
       <ul>
           <li><strong>C </strong></li>
           <li><strong>Python</strong></li>
           <li><strong>Java </strong></li>
        </ul>
    </div>
</div>
{/if}
{#if togglefront}
<div class="card-front">
    <div>
       <ul>
           <li><strong>HTML</strong></li>
           <li><strong>CSS</strong></li>
           <li><strong>JavaScript</strong></li>
           <li><strong>ReactJS</strong></li>
           <li><strong>Svelte</strong></li>
        </ul>
    </div>
</div>
{/if}
{#if toggleback}
<div class="card-back">
    <div>
       <ul>
           <li><strong>NodeJs</strong></li>
           <li><strong>ExpressJS</strong></li>
           
        </ul>
    </div>
</div>
{/if}
{#if toggledata}
<div class="card-data">
    <div>
       <ul>
           <li><strong>MSSQL</strong></li>
           <li><strong>MongoDB</strong></li>
           
        </ul>
    </div>
</div>
{/if}
{#if toggletest}
<div class="card-test">
    <div>
       <ul>
           <li><strong>Junit</strong></li>
           <li><strong>Selenium</strong></li>
           <li><strong>TestNG</strong></li>
           <li><strong>Cucumber</strong></li>
           <li><strong>ReadyAPI</strong></li>
           <li><strong>Appium (Mobile App Testing)</strong></li>
        </ul>
    </div>
</div>
{/if}
{#if togglemanage}
<div class="card-manage">
    <div>
       <ul>
           <li><strong>GitHub</strong></li>
           <li><strong>JIRA</strong></li>
           <li><strong>Jenkins</strong></li>
        </ul>
    </div>
</div>
{/if}
</body>
<style>
    body {
        margin: 0;
        height: 100vh; 
        overflow-y: auto; 
        flex-wrap: wrap; 
}
    .card-programming{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 50%;
        height : 15%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-image: url('http://images.unsplash.com/photo-1523878288860-7ad281611901?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8Mnx8cG9ydGZvbGlvJTIwYmFja2dyb3VuZHx8MHx8fHwxNjIxNjIxNDk3&ixlib=rb-1.2.1&q=80&w=1080');
        background-size: cover;
        background-repeat: no-repeat;
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-front{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 50%;
        height : 25%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-image: url('http://images.unsplash.com/photo-1523878288860-7ad281611901?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8Mnx8cG9ydGZvbGlvJTIwYmFja2dyb3VuZHx8MHx8fHwxNjIxNjIxNDk3&ixlib=rb-1.2.1&q=80&w=1080');
        background-size: cover;
        background-repeat: no-repeat;
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-back{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 50%;
        height : 15%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-image: url('http://images.unsplash.com/photo-1523878288860-7ad281611901?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8Mnx8cG9ydGZvbGlvJTIwYmFja2dyb3VuZHx8MHx8fHwxNjIxNjIxNDk3&ixlib=rb-1.2.1&q=80&w=1080');
        background-size: cover;
        background-repeat: no-repeat;
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-data{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 50%;
        height : 15%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-image: url('http://images.unsplash.com/photo-1523878288860-7ad281611901?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8Mnx8cG9ydGZvbGlvJTIwYmFja2dyb3VuZHx8MHx8fHwxNjIxNjIxNDk3&ixlib=rb-1.2.1&q=80&w=1080');
        background-size: cover;
        background-repeat: no-repeat;
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-test{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 15%;
        position: absolute;
        top : 50%;
        height : 25%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-image: url('http://images.unsplash.com/photo-1523878288860-7ad281611901?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8Mnx8cG9ydGZvbGlvJTIwYmFja2dyb3VuZHx8MHx8fHwxNjIxNjIxNDk3&ixlib=rb-1.2.1&q=80&w=1080');
        background-size: cover;
        background-repeat: no-repeat;
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-manage{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 50%;
        height : 15%;
        width : 15%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-image: url('http://images.unsplash.com/photo-1523878288860-7ad281611901?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8Mnx8cG9ydGZvbGlvJTIwYmFja2dyb3VuZHx8MHx8fHwxNjIxNjIxNDk3&ixlib=rb-1.2.1&q=80&w=1080');
        background-size: cover;
        background-repeat: no-repeat;
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .btns{ 
        margin-top : 5%;
        margin-left : 2%;
    }

    .btns button{
        display: flex;
        align-items: center;
        justify-content: center;
        line-height: 1;
        text-decoration: none;
        color: #333333;
        font-size: 18px;
        border-radius: 0px;
        width: 200px;
        height: 40px;
        font-weight: bold;
        border: 2px solid #333333;
        transition: 0.3s;
        box-shadow: 5px 5px 0px 0px rgba(51, 51, 51, 1);
        background-color: #52b35e;
    }
    .btns button:hover{
        box-shadow: 0 0 #333;
        color: #fff;
        background-color: #333;
    }

@media (max-width: 768px) {
    .btns {
        position: absolute; 
        top: 30%;
        right: 80%;
    }

    .btns button {
        font-size: 15px; 
        width: 150px; 
        height: 42px; 
    }

    .card-programming, .card-front, .card-back, .card-data, .card-manage {
        max-width: 30%; 
        height: 15%;
        position: absolute;
        top: 35%;
        right: 55%;
    }
    .card-test{
        max-width: 30%; 
        height: 20%;
        position: absolute;
        top: 35%;
        right: 55%;
    }

}

@media (max-width: 480px) {
    .btns {
        top: 30%;
        right: 55%;
    
         
    }

    .btns button {
        font-size: 12px; 
        width: 130px; 
        height: 30px; 
        margin-bottom: 5px;
    }

    .card-programming{
        width: 50%; 
        max-height: 13%;
        right: 10%; 
        top: 32%; 

    } .card-front{
        width: 50%; 
        max-height: 15%;
        right: 7%; 
        top: 33%; 
    } 
    .card-back{
        width: 50%; 
        max-height: 10%;
        right: 0%; 
        top: 33%; 
    } 
    .card-data{
        width: 45%; 
        max-height: 10%;
        right: 2%; 
        top: 33%; 

    } 
    .card-manage {
        width: 50%;
        max-height: 15%;
        right: 0%; 
        top: 30%;
    }
    .card-test{
        max-width:20%;
        height: 20%;
        right: 18%; 
        top: 30%;
    }    
}

</style>
