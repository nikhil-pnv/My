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
    height: 100vh; /* Setting the body height to the viewport height */
    overflow-y: auto; /* If content exceeds the viewport height, make it scrollable */
    flex-wrap: wrap; /* Wrap the flex items if there isn't enough space */
}


.card {
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    max-width: 600px;
    margin: 20px auto; /* Added vertical margin for spacing */
    text-align: left; 
    background-color: rgba(182, 195, 222, 0.75);
    line-height: 1.6;
    backdrop-filter: blur(16px) saturate(180%);
}

button {
    padding: 10px 15px;
    margin: 5px;
    font-size: 16px;
    cursor: pointer; /* Indicates clickable items */
    transition: background-color 0.3s; /* Background transition effect on hover */
}

button:hover {
    background-color: green; /* Change background color on hover */
}

/* For tablets and smaller devices */
@media (max-width: 768px) {

    .card {
        max-width: 90%;
        padding: 15px;
        margin-top: 1%;
    }

    button {
        padding: 8px 12px;
        font-size: 14px;
    }
}

/* For mobile devices */
@media (max-width: 480px) {
    .card {
        max-width: 100%;
        padding: 10px;
        margin-top: 5%;
    }

    button {
        padding: 6px 10px;
        font-size: 12px;
        margin: 5px;
    }
}

  
</style>
