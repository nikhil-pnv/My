<script>
    let togglebtech = false;
    let toggleten = false;
    let toggleinter = false;

    function tenthInfo(){
        togglebtech = false;
        toggleten = true;
        toggleinter = false;
    }

    function btechInfo(){
        togglebtech = true;
        toggleten = false;
        toggleinter = false;
    }
    function interInfo(){
        togglebtech = false;
        toggleten = false;
        toggleinter = true;
    }

   
</script>
{#if toggleten}
<div class="card">
    <div>
       <ul>
           <li><strong>Narayana High School, Anakapalle</strong></li>
           <li><strong>Year :</strong> 2016 - 2017</li>
           <li><strong>Board :</strong> Andhra Pradesh Board of Intermediate</li>
           <li><strong>CGPA :</strong> 10.0</li>

        </ul>
    </div>
</div>
{/if}
{#if togglebtech}
<div class="card">
     <div>
        <ul>
            <li><strong>Vignan's Institute of Information and Technology, Visakhapatnam</strong></li>
            <li><strong>Year :</strong> 2019 - 2023</li>
            <li><strong>Branch :</strong> Computer Science and Engeneering (CSE)</li>
            <li><strong>CGPA :</strong> 8.45</li>

         </ul>
     </div>
</div>
{/if}
{#if toggleinter}
<div class="card">
    <div>
       <ul>
           <li><strong>Sri Chaitanya Junior college, Ukkunagaram</strong></li>
           <li><strong>Year :</strong> 2017 - 2019</li>
           <li><strong>Stream :</strong> M.P.C</li>
           <li><strong>Percentage :</strong> 96</li>

        </ul>
    </div>
</div>
{/if}

<div class="btns">
    <button on:click={tenthInfo}><strong>Tenth</strong></button><br><br><br><br><br>
    <button on:click={interInfo}><strong>Intermediate</strong></button><br><br><br><br><br>
    <button on:click={btechInfo}><strong>B-Tech</strong></button>
</div>

<style>
    .card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    transition: 0.3s;
    width: 40%;
    max-width: 400px; /* set a max-width so it doesn't get too wide on large screens */
    margin: 2rem auto; /* centers the card horizontally and provides vertical spacing */
    backdrop-filter: blur(16px) saturate(180%);
    -webkit-backdrop-filter: blur(16px) saturate(180%);
    background-color: rgba(182, 195, 222, 0.75);
    border-radius: 12px;
    border: 1px solid rgba(255, 255, 255, 0.125);
    position: relative; /* this makes it a reference point for the absolute positioned child elements */
}

.btns {
    display: flex;
    gap: 1rem;
    margin-top: 2rem;
    justify-content: center;
}

.btns button {
    display: flex;
    align-items: center;
    justify-content: center;
    line-height: 1;
    text-decoration: none;
    color: #333333;
    font-size: 1rem;
    border-radius: 0px;
    width: 200px;
    height: 40px;
    font-weight: bold;
    border: 2px solid #333333;
    transition: 0.3s;
    box-shadow: 5px 5px 0px 0px rgba(51, 51, 51, 1);
    background-color: #52b35e;
}

.btns button:hover {
    box-shadow: 0 0 #333;
    color: #fff;
    background-color: #333;
}
/* For tablets and smaller devices */
/* ... Previous CSS styles ... */

@media (max-width: 768px) {
    .card {
        width: 80%;
        position: absolute;
        top : 75%;
        right: 20%;
        margin: 2rem auto; /* Use margins to provide spacing */
    }

    .btns {
        margin-top: 0rem;
        gap: 1rem;
        flex-direction: column; /* Stack buttons vertically */
        position: absolute;
        top : 75%;
    }

    .btns button {
        width: 140px;
        font-size: 0.8rem;
    }
}


@media (max-width: 480px) {
    .btns {
        flex-direction: column;
        gap: 1rem;
        margin-top: 3rem;  /* Use margins instead of positioning */
    }

    .btns button {
        width: 90px;
        font-size: 0.7rem;
    }

    .card{
        width: 70%;
        margin-top: 5rem ;  
        right: 5%;
    }
}


</style>