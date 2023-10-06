<script>
    import { fly } from 'svelte/transition';

    let projects = [
        '<ul><li><strong>Project Name</strong>: Blog Website </li> <li><strong>Tech Stacks</strong> : HTML, CSS, JavaScript, ReactJs, NodeJs, MongoDB, ExpressJs </li><li><strong>Description</strong> : Developed a blogging website that allows users to create their own blog and users can publish their thoughts which can be read by all the users.</li> <li><strong>Repository</strong> : <a href="https://github.com/nikhil-pnv/BlogApp">source code</a></li></ul>',
        '<ul><li><strong>Project Name</strong>: Food Recipes </li> <li><strong>Tech Stacks</strong> : HTML, CSS, JavaScript, ReactJs, NodeJS, API Calls, MealDB API </li><li><strong>Description</strong> : This website is designed using reactjs and API calls where users can find recipes and related video of foof items recipes.</li> <li><strong>Repository</strong> : <a href="https://github.com/nikhil-pnv/FoodRecipe">source code</a></li> <li><strong>Project Link</strong> : <a href="https://pnv-food-recipe.netlify.app"> click here</a></li></ul>',
        '<ul><li><strong>Project Name</strong>: Automatic Railway Gates </li> <li><strong>Materials Used</strong> : Arduino Board, IR Sensors, Servo Motors</li><li><strong>Software</strong>: Arduino programming</li><li><strong>Description</strong> : This project detects the train and automatically open and close the railway gates upon detecting the arrival or departure of train.</li></ul>',

       ];

    let currentCard = 0;

    function nextCard() {
        if (currentCard < projects.length - 1) {
            currentCard++;
        }
    }

    function prevCard() {
        if (currentCard > 0) {
            currentCard--;
        }
    }
</script>
<body>
{#if currentCard !=0}
<button on:click={prevCard}>&lt; Prev</button>
{/if}
<div 
    class="card"
    in:fly={{ x: 200, duration: 300 }}
    out:fly={{ x: -200, duration: 300 }}
>
    {@html projects[currentCard]}
</div>
{#if currentCard != projects.length-1}
<button on:click={nextCard}>Next &gt;</button>
{/if}
</body>
<style>
    body { 
    margin: 0;
    padding-top: 1%;
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 100vh; 
    overflow-y: auto; 
    flex-wrap: wrap;
}


.card {
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    max-width: 600px;
    margin: 20px auto;
    text-align: left; 
    background-image: url('http://images.unsplash.com/photo-1523878288860-7ad281611901?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8Mnx8cG9ydGZvbGlvJTIwYmFja2dyb3VuZHx8MHx8fHwxNjIxNjIxNDk3&ixlib=rb-1.2.1&q=80&w=1080');
        background-size: cover;
        background-repeat: no-repeat;
    line-height: 1.6;
    backdrop-filter: blur(16px) saturate(180%);
    margin-left: 5%;
    margin-top: 4%;
}

button {
    padding: 10px 15px;
    margin: 5px;
    font-size: 16px;
    margin-left: 1%;
    cursor: pointer; 
    transition: background-color 0.3s; 
}

button:hover {
    background-color: green; 
}


@media (max-width: 768px) {

    .card {
        max-width: 30%;
        padding: 15px;
        margin-top: 1%;
    }

    button {
        padding: 8px 12px;
        font-size: 14px;
    }
}

@media (max-width: 480px) {
    .card {
        max-width: 40%;
        padding: 10px;
        margin-top: 13%;
        margin-left: 1%;
    }

    button {
        padding: 6px 10px;
        font-size: 12px;
        margin: 5px;
    }
}
  
</style>
