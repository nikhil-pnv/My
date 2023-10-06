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
    <img src="https://media2.giphy.com/media/dWesBcTLavkZuG35MI/giphy.gif?cid=ecf05e473cp9lm2c2qafqqv1y0z60x4k4xhxf2883t3hpc61&ep=v1_gifs_related&rid=giphy.gif&ct=g" alt="GIF"/>
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
    background-color: #eaeff2; 
    margin: 0; 
    font-family: Arial, sans-serif;
    scroll-behavior: auto; 
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
        margin-left: 87%;
        top : 0%;
    }
    .gif img {
        position:absolute;
        width: 15vh;  
        height: 14vh;
        right: -8vh;
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
      margin-top: 0.5vh;
      left: -5%;
    }

    .gif img {
        position: absolute;
        height: 11vh;
        width: 12vh;  
    }
}
</style>
