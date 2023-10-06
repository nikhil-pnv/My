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
        overflow-y: auto; 
        flex-wrap: wrap; 
        scroll-behavior: auto;
    }
    .btns{ 
        position: absolute;
        right : 80%;
        margin-top: 4%;
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
        top : 28%;
        height : 7%;
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
    .card-linkedin{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 40%;
        height : 7%;
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
    .card-gmail{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 52%;
        height : 7%;
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
    .card-insta{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 63%;
        height : 7%;
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
    .card-facebook{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 75%;
        height : 7%;
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
    .card-contact{
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        position: absolute;
        top : 88%;
        height : 7%;
        width : 20%;
        right : 50%;
        background-image: url('http://images.unsplash.com/photo-1523878288860-7ad281611901?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8Mnx8cG9ydGZvbGlvJTIwYmFja2dyb3VuZHx8MHx8fHwxNjIxNjIxNDk3&ixlib=rb-1.2.1&q=80&w=1080');
        background-size: cover;
        background-repeat: no-repeat;
        backdrop-filter: blur(16px) saturate(180%);
        -webkit-backdrop-filter: blur(16px) saturate(180%);
        border-radius: 12px;
        border: 1px solid rgba(255, 255, 255, 0.125);
    }

    @media (max-width: 768px) {
    .btns {
        position: absolute; 
        top: 35%;
        right: 85%; 
    }

    .btns button {
        font-size: 0.8rem; 
        width: 90%; 
        height: 90%; 

    }

    .card-git{
        width: 18%; 
        position: absolute;
        top: 38%;
        font-size: 0.8rem;
        right: 58%;
        height: 5%;
    }
    .card-linkedin{
        width: 20%; 
        position: absolute;
        font-size: 0.8rem;
        top: 43%;
        right: 58%;
        height: 5%;
    }
    .card-gmail{
        width: 30%; 
        position: absolute;
        font-size: 0.7rem;
        top: 50%;
        right: 54%;
        height: 4%;

    }
    .card-insta{
        width: 20%; 
        position: absolute;
        font-size: 0.8rem;
        top: 56%;
        right: 58%;
        height: 4%;

    }
    .card-facebook{
        width: 20%; 
        position: absolute;
        font-size: 0.8rem;
        top: 62%;
        right: 61%;
        height: 4%;
    }
    .card-contact {
        width: 20%; 
        position: absolute;
        font-size: 0.8rem;
        top: 68%;
        right: 60%; 
        height: 4%;
    }

}

@media (max-width: 480px) {
    .btns {
        top: 30%;
        right: 75%;
        gap: 0.5rem;
        
    }

    .btns button {
        font-size: 10px; 
        width: 90%; 
        height: 30px;
        margin-bottom: 5px; 
    }

    .card-git{
        font-size: 0.7rem;
        width: 40%; 
        height: 4%;
        right: 10%; 
        top: 35%;
    } 
    .card-linkedin{
        font-size: 0.7rem;
        width: 50%; 
        height: 4%;
        right: 7%; 
        top: 35%; 
    } 
    .card-gmail{
        font-size: 0.7rem;
        width: 65%; 
        height: 4%;
        right: 5%; 
        top: 35%; 
    }
    .card-insta{
        font-size: 0.7rem;
        width: 52%; 
        height: 4%;
        right: 10%; 
        top: 35%; 
    }
    .card-facebook{
        font-size: 0.7rem;
        width: 55%; 
        height: 4%;
        right: 10%; 
        top: 35%; 
    }
    .card-contact {
        font-size: 0.7rem;
        width: 50%; 
        height: 4%;
        right: 10%; 
        top: 35%; 
    }
    
}

</style>
