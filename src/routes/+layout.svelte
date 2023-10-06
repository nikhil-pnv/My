<script>
    import src from '../mypic.png';

</script>
<body>
<div class="container">
    <div class="name">
        <p>&nbsp; PORTFOLIO &nbsp;&nbsp;</p>
    </div>
    <div class="navbar">
        <nav>
          <a href="/about">About</a>
          <a href="/education" >Education</a>
          <a href="/skills">Skills</a>
          <a href="/projects">Projects</a>
          <a href="/connect">Connect</a>
        </nav>
      </div>
</div>
<div class="mypic">
    <img {src} alt="A portrait of me"/>
</div>   
<div class="gif">
    <img src="https://raw.githubusercontent.com/punitkmryh/punitkmryh/master/Developer.gif" alt="GIF"/>
</div>
 
</body>
  
  <slot /> 
  
<style>
    *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    }
    body { 
    /*background-image: url('http://images.unsplash.com/photo-1470790376778-a9fbc86d70e2?ixlib=rb-1.2.1&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=1080&fit=max&ixid=eyJhcHBfaWQiOjEyMDd9');
    background-repeat: no-repeat;*/
    background-size: cover;
    margin: 0; 
    font-family: Arial, sans-serif;
}

.container {
    display: flex;
    margin : 0;
    flex-direction: column;
    align-items: center; 
    justify-content: center;
    gap: 30px; 
    margin-top: 1%;
    
}
.gif{
    position: absolute;
    top : 30%;
    margin-left: 1%;
    right: 0%;
}

.gif img {
    border-radius: 30%;
    height: 60vh ;
    width: 90vh;
    

}
.mypic{
    position: absolute;
    top : 1%;
}

.mypic img {
    width: 25vh;
    height: 25vh;
    border-radius: 50%;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);  
    background: #acd2cc;
    
}

.name { 
    background: #deac61;
    text-align: center;
    width: 100%;
}

.name p {
    color: #2709ef;
    padding: 10px 0;
}

.navbar {
    display: flex;
    align-items: center; 
    background: #deac61;
    width: 100%;
}

nav {
    display: flex;
    gap: 20px;  
    padding: 10px; 
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); 
    flex: 1;
    justify-content: center; 
}

nav a {
    text-decoration: none;  
    color: rgb(52, 5, 238); 
    padding: 5px 15px;
    border-radius: 10px;
    transition: background-color 0.2s; 
}

nav a:hover {
    background-color: #bbf793;
}

@media (max-width: 768px), (max-height : 500px) {
    .name{
        width: 100%;
    }
    .name p{
        font-size: 1rem;
        text-align: center;
    }
    nav {
        flex-direction: column;
        gap: 10px;
    }
    nav a{
        text-align: center;
    }
    .navbar{
        width: 100%;
    }
    .mypic{
        margin-left: 18%;
        top : 0%;
    }

    .mypic img {
        position: absolute;
        right : 80%;
        top: 23%;
        width: 16vh;
        height: 14vh;
    }
    .gif{
        position: absolute;
        right: 50%;
        top : 38%;

    }
    .gif img {
        position:absolute;
        width: 50vh;  
        height: 35vh;
    }
}


@media (max-width: 480px) {
      
    .name{
        width: 110%;
    }
    .name p{
        font-size: 0.9rem;
        text-align: center;
    }
    .navbar{
        width: 110%;
    }
    nav{
        flex-direction: column;
        gap: 8px;  
    }
    nav a{
        text-align: center;
    }
    .mypic{
        top: 0.5%;
        margin-left: 30%;
    }

    .mypic img {
        position: absolute;
        margin-top: 20%; 
        width: 11vh;  
        height: 12vh;  
    }
    .gif{
      position: absolute;
      top: 47%;
      right: 84%;
    }

    .gif img {
        position: absolute;
        height: 25vh;
        width: 30vh;  
    }
}

</style>
