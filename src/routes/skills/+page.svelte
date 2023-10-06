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
           <li><strong>C programming</strong></li>
           <li><strong>Python</strong></li>
           <li><strong>Java Basics</strong></li>
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
        overflow-y: auto; /* If content exceeds the viewport height, make it scrollable */
        flex-wrap: wrap; 
}
    .card-programming{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 130%;
        height : 15%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-front{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 130%;
        height : 25%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-back{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 130%;
        height : 15%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-data{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 130%;
        height : 15%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-test{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 15%;
        position: absolute;
        top : 130%;
        height : 25%;
        width : 20%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-manage{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        width: 40%;
        position: absolute;
        top : 130%;
        height : 15%;
        width : 15%;
        right : 50%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .btns{ 
        margin-top : 0%;
        right : 85%;
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

    /* ... Your existing CSS styles ... */

/* For tablets and smaller devices */
@media (max-width: 768px) {
    .btns {
        position: absolute; /* Adjusted position */
        top: 75%;
        right: 75%; /* Adjusted position */
    }

    .btns button {
        font-size: 15px; /* Smaller font size */
        width: 150px; /* Adjusted width */
        height: 42px; /* Adjusted height */
    }

    .card-programming, .card-front, .card-back, .card-data, .card-test, .card-manage {
        width: 50%; /* Increase width to utilize space */
        position: absolute;
        top: 95%;
        right: 15%; /* Center the card */
    }

}

/* For mobile devices */
@media (max-width: 480px) {
    .btns {
        top: 90%;
        right: 70%;
        flex-direction: column; /* Stack buttons vertically */
    }

    .btns button {
        font-size: 12px; /* Even smaller font size */
        width: 130px; /* Adjusted width */
        height: 30px; /* Adjusted height */
        margin-bottom: 5px; /* Add some space between stacked buttons */
    }

    .card-programming, .card-front, .card-back, .card-data, .card-manage {
        width: 50%; /* Almost full width */
        height: 40%;
        right: 2%; /* Center the card */
        top: 120%; /* Adjusted top position */
    }
    .card-test{
        width : -10%;
        height: 50%;
        right: 0%; /* Center the card */
        top: 120%;
    }

    
}

</style>