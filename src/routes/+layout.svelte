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
    <div class="gif">
        <img src="https://media2.giphy.com/media/dWesBcTLavkZuG35MI/giphy.gif?cid=ecf05e473cp9lm2c2qafqqv1y0z60x4k4xhxf2883t3hpc61&ep=v1_gifs_related&rid=giphy.gif&ct=g" alt="GIF"/>
    </div>
    <div class="mypic">
      <img {src} alt="A portrait of me"/>
    </div>
    
    
  
    
</div>
 
</body>
  
  <slot /> 
  
<style>
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
    min-height: 100vh; 
    gap: 30px; 
    
}

.gif img {
    border-radius: 30%;
    max-width: 100%; 
    height: auto ;
    width: 70%;
    margin-left: auto;
    margin-right: auto;
}

.mypic img {
    width: 180px;
    height: 180px;
    border-radius: 50%;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);  
    background: #acd2cc;
    position: absolute;
    top : 10%;
    left: 5%;
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

@media (max-width: 768px) {
    nav {
        flex-direction: column;
        gap: 10px;
    }

    .mypic img {
        position: absolute;
        right : 80%;
        top: 23%;
        width: 120px;
        height: 110px;
    }
    .gif img {
        position:absolute;
        width: 150px;  
        height: 110px;
        right: 8%;
        bottom : 63%;
    }
}


@media (max-width: 480px) {
    nav {
        flex-direction: column;
        gap: 8px;  
    }

    .mypic img {
        position: absolute;
        left: 2%;  
        top: 11%; 
        width: 100px;  
        height: 95px;  
    }

    .gif img {
        position: absolute;
        height: 20%;
        width: 25%; 
        right: 3%;  
        bottom: 70%; 
    }
}



</style>
