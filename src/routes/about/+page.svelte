<script>
    let aboutText = "&nbsp;&nbsp;&nbsp;&nbsp; <strong>Hi ! I'm  NIKHIL VARMA PINNAMARAJU </strong> <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp<strong>Full Stack Developer and Tester.</strong><br>I'm a dedicated Full Stack Developer with strong proficiency in Python, Java, C programming languages. As a passionate computer science graduate, I have acquired strong skills in frontend technologies such as HTML, CSS, JavaScript and frontend frameworks such as ReactJS, Svelte and backend as NodeJs and testing frameworks such as Junit, Selenium, TestNG, Appium, alongside a solid foundation in database management, particularly in MSSQL and MongoDB. I believe in continuous learning and adaptation, striving always to stay updated with the latest in technology and design trends.";
</script>
<body>
<div class="container">
    <p class="about">ABOUT</p>
    <div class="card">
        <div class="text">
            <p>{@html aboutText}</p>
        </div>
    </div>
</div>
</body>
<style>
    body {
    margin: 0;
    height: 100vh;
    overflow-y: auto;
    flex-wrap: wrap;
}

.container {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.about {
    text-align: center;
    font-size: 2rem;
    font-weight: bold;
    color: blue;
    position: absolute;
    right: 60%;
    top: 25%;
}

.text p {
    line-height: 1.6;
    word-spacing: 0.2em;
    color: rgb(252, 44, 7);
    font-weight: bolder;
    padding: 1rem;
}

.card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    transition: 0.3s;
    width: 50%;
    backdrop-filter: blur(16px) saturate(180%);
    -webkit-backdrop-filter: blur(16px) saturate(180%);
    background-image: url('http://images.unsplash.com/photo-1523878288860-7ad281611901?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8Mnx8cG9ydGZvbGlvJTIwYmFja2dyb3VuZHx8MHx8fHwxNjIxNjIxNDk3&ixlib=rb-1.2.1&q=80&w=1080');
    background-size: cover;
    background-repeat: no-repeat;
    border-radius: 12px;
    border: 1px solid rgba(255, 255, 255, 0.125);
    margin-top: 1%;
    position: absolute;
    right: 40%;
    top: 40%;
}

.card:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
}

@media (max-width: 768px) {
    .about {
        font-size: 1.5rem;
        position: absolute;
        top: 30%;
        right: 45%;
    }

    .card {
        position: absolute;
        top: 39%;
        width: 100%;
        left: 5%;
    }
}

@media (max-width: 480px) {
    .about {
        font-size: 1rem;
        margin-top: 9%;
        position: absolute;
        top: 30%;
        left: 40%;
    }

    .card {
        width: 95%;
        position: absolute;
        top: 35%;
        left: 3%;
    }
}

</style>
