<script>
    let aboutText = "&nbsp;&nbsp;&nbsp;&nbsp; <strong>Hi ! I'm  NIKHIL VARMA PINNAMARAJU </strong> <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp<strong>Full Stack Developer and Tester.</strong><br>I'm a dedicated Full Stack Developer with strong proficiency in Python, Java, C programming languages. As a passionate computer science graduate, I have acquired strong skills in frontend technologies such as HTML, CSS, JavaScript and frontend frameworks such as ReactJS, Svelte and backend as NodeJs and testing frameworks such as Junit, Selenium, TestNG, Appium, alongside a solid foundation in database management, particularly in MSSQL and MongoDB. I believe in continuous learning and adaptation, striving always to stay updated with the latest in technology and design trends.";
</script>
<body>
<div class="container">
    <p class="about">About Me</p>
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
    margin-top: 1%;
    font-size: 2rem;
    font-weight: bold;
    color: blue;
}

.text p {
    line-height: 1.6;
    word-spacing: 0.2em;
    color: rgb(229, 73, 11);
    padding: 1rem;
}

.card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    transition: 0.3s;
    width: 50%;
    backdrop-filter: blur(16px) saturate(180%);
    -webkit-backdrop-filter: blur(16px) saturate(180%);
    background-color: rgba(182, 195, 222, 0.75);
    border-radius: 12px;
    border: 1px solid rgba(255, 255, 255, 0.125);
    margin-top: 1%;
}

.card:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
}

/* Responsive styles */
@media (max-width: 768px) {
    .about {
        font-size: 1.5rem;
        position: absolute;
        top: 70%;
    }

    .card {
        position: absolute;
        top: 80%;
        width: 80%;
    }
}

@media (max-width: 480px) {
    .about {
        font-size: 1.2rem;
        margin-top: 6%;
    }

    .card {
        width: 90%;
        margin-top: 3%;
    }
}

</style>
