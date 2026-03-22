<center><h1>Welcome to my very kind and cute ToDo Appi!</h1></center>


<style>
   p {
        font-family: cursive;
        color: #fef9ff;
        font-size: 18px;
        font-weight: bolder;
    }



    h1 {
        font-family: cursive;
        color: #fef9ff;
        border-style: inset;
        border-color: #fef9ff;
        border-width: 5px;
        text-align: center;
        border-spacing: 10;
        text-decoration-line: underline;
        background-color: #ffb5a7;
        width: 800px;
        text-size-adjust: 100px;

    }

    .background-div {
        position: fixed; /* Fixes the div to the viewport, even on scroll */
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: -1; /* Pushes the div behind all other content */
        background-image: url(/flowers.jpg);
    }

    .div-regular {
        background-color: #ffb5a7;
        width: 800px;
        height: 1000px;
        border-style: inset;
        border-color: #fef9ff;
        border-width: 5px;
        
    }

    button {
       margin: 75px 0px 25px 500px; 
       background-color: #ff9782;
       width: 70px;
       height: 45px;
       border-style: inset;
       border-color: #fef9ff;
       border-width: 5px;
       text-decoration: none;
  /* Centers text horizontally */
        text-align: center;
    }

    input {
        background-color: #ff9782;
        border-style: inset;
        border-color: #fef9ff;
        border-width: 5px;
        width: 200px;
        height: 25px;
        font-family: cursive;
        color: #fef9ff;
        font-size: large;
    }

    .box {
        border-style: inset;
       border-color: #fef9ff;
       border-width: 5px;
       font-family: cursive;
       color: #fef9ff;
       font-size: large;
       padding: 25px 200px 25px 200px;
       text-align: right;
       align-items: right;
    }
</style>

<script>

    let count = $state(0);
    let task = $state();

    function addTask () {
        console.log('hi')
        count += 1;
    }
</script>

<div class="background-div">
</div> 
<center>
    <div class="div-regular"> 
        <input bind:value={task} placeholder="input task here"/>
        <button onclick={addTask}>
            <p>add task</p>
        </button>
            <h1>Task: {task}</h1>
            <box class='box'>this is my beautiful bountiful box</box>
    </div> 
    
    
</center>  





