<script>
    let toggleGit =false;
    let toggleLinkedin =false;
    let toggleMail =false;
    let toggleInsta =false;
    let toggleFacebook =false;
    let toggleContact=false;
    function gitConnect(){
        toggleGit = true;
        toggleLinkedin =false;
        toggleMail =false;
        toggleInsta =false;
        toggleFacebook =false;
        toggleContact=false;

    }
    function linkedinConnect(){
        toggleGit = false;
        toggleLinkedin =true;
        toggleMail =false;
        toggleInsta =false;
        toggleFacebook =false;
        toggleContact=false;
    }
    function mailConnect(){
        toggleGit = false;
        toggleLinkedin =false;
        toggleMail = true;
        toggleInsta =false;
        toggleFacebook =false;
        toggleContact=false;

    }
    function instaconnect(){

        toggleGit = false;
        toggleLinkedin =false;
        toggleMail =false;
        toggleInsta =true;
        toggleFacebook =false;
        toggleContact=false;
    }
    function facebookConnect(){
        toggleGit = false;
        toggleLinkedin =false;
        toggleMail =false;
        toggleInsta =false;
        toggleFacebook = true;
        toggleContact=false;

    }
    function contactConnect(){
        toggleGit = false;
        toggleLinkedin =false;
        toggleMail =false;
        toggleInsta =false;
        toggleFacebook = false;
        toggleContact = true;
    }
    
</script>
<body>
    <div class="btns">
        <button on:click={gitConnect}><strong>GitHub</strong></button><br><br>
        <button on:click={linkedinConnect}><strong>LinkedIn</strong></button><br><br>
        <button on:click={mailConnect}><strong>Gmail</strong></button><br><br>
        <button on:click={instaconnect}><strong>Instagram</strong></button><br><br>
        <button on:click={facebookConnect}><strong>Facebook</strong></button><br><br>
        <button on:click={contactConnect}><strong>Contact</strong></button><br><br>
    
    </div>
{#if toggleGit}
<div class="card-git">
    <div>
       <ul>
           <li><a href="https://github.com/nikhil-pnv"><strong>GitHub Profile</strong></a></li>
        </ul>
    </div>
</div>
{/if}
{#if toggleLinkedin}
<div class="card-linkedin">
    <div>
       <ul>
        <li><a href="https://www.linkedin.com/in/nikhil-varma-pinnamaraju-3464a3205?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app "><strong>LinkedIn Profile</strong></a></li>
    </ul>
    </div>
</div>
{/if}
{#if toggleMail}
<div class="card-gmail">
    <div>
       <ul>
           <li><p><strong>nikhilvarma1810@gmail.com</strong></p></li>
        </ul>
    </div>
</div>
{/if}
{#if toggleInsta}
<div class="card-insta">
    <div>
       <ul>
        <li><a href="https://www.instagram.com/p____n____v/?igshid=MzMyNGUyNmU2YQ%3D%3D"><strong>Instagram Profile</strong></a></li>
    </ul>
    </div>
</div>
{/if}
{#if toggleFacebook}
<div class="card-facebook">
    <div>
       <ul>
        <li><a href="https://www.facebook.com/nikhilvarma.pinnamaraju?mibextid=ZbWKwL"><strong>Facebook Profile</strong></a></li>
    </ul>
    </div>
</div>
{/if}
{#if toggleContact}
<div class="card-contact">
    <div>
       <ul>
           <li><p><strong>+91 9573012245</strong></p></li>
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
    .btns{ 
        position: absolute;
        right : 60%;
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
    .card-git{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 99%;
        height : 7%;
        width : 20%;
        right : 30%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-linkedin{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 111%;
        height : 7%;
        width : 20%;
        right : 30%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-gmail{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 124%;
        height : 7%;
        width : 20%;
        right : 30%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-insta{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 137%;
        height : 7%;
        width : 20%;
        right : 30%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-facebook{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 150%;
        height : 7%;
        width : 20%;
        right : 30%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }
    .card-contact{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 163%;
        height : 7%;
        width : 20%;
        right : 30%;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        background-color: rgba(182, 195, 222, 0.75);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }

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

    .card-git{
        width: 23%; /* Increase width to utilize space */
        position: absolute;
        top: 74%;
        right: 35%;
        height: 6%;
    }
    .card-linkedin{
        width: 23%; /* Increase width to utilize space */
        position: absolute;
        top: 84%;
        right: 35%;
        height: 6%;
    }
    .card-gmail{
        width: 35%; /* Increase width to utilize space */
        position: absolute;
        top: 95%;
        right: 30%;
        height: 6%;

    }
    .card-insta{
        width: 25%; /* Increase width to utilize space */
        position: absolute;
        top: 105%;
        right: 35%;
        height: 6%;

    }
    .card-facebook{
        width: 25%; /* Increase width to utilize space */
        position: absolute;
        top: 115%;
        right: 35%;
        height: 6%;
    }
    .card-contact {
        width: 25%; /* Increase width to utilize space */
        position: absolute;
        top: 125%;
        right: 35%; /* Center the card */
        height: 6%;
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

    .card-git{
        width: 40%; /* Almost full width */
        height: 8%;
        right: 10%; /* Center the card */
        top: 89%; /* Adjusted top position */
    } 
    .card-linkedin{
        width: 40%; /* Almost full width */
        height: 8%;
        right: 10%; /* Center the card */
        top: 103%; /* Adjusted top position */
    } 
    .card-gmail{
        width: 60%; /* Almost full width */
        height: 8%;
        right: 2%; /* Center the card */
        top: 118%; /* Adjusted top position */
    }
    .card-insta{
        width: 40%; /* Almost full width */
        height: 8%;
        right: 10%; /* Center the card */
        top: 133%; /* Adjusted top position */
    }
    .card-facebook{
        width: 40%; /* Almost full width */
        height: 8%;
        right: 10%; /* Center the card */
        top: 148%; /* Adjusted top position */
    }
    .card-contact {
        width: 40%; /* Almost full width */
        height: 8%;
        right: 10%; /* Center the card */
        top: 163%; /* Adjusted top position */
    }
    
}



</style>
