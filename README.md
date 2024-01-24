# Simple-calculator
Calculator website 
<!DOCTYPE html>
<html lang="en"><!--Performing some styles for certain attributes within the code--><head><style>
    p,
    h1 {

        text-align: center;
    }

    body {

        background-color: turquoise;
    }

    .button {
        text-align: center;
    }

    .button input[type="button"] {
        background-color: #eab676;
        color: aliceblue;
    }
</style>


<script>


    function add() {

        let numberOne = prompt("Enter number one:");

        let numberTwo = prompt("Enter number two:");

        sum = Number(numberOne) + Number(numberTwo);

        let resultBody = document.createElement("p");

        resultBody.textContent = `${numberOne} + ${numberTwo} = ${sum}`;

        document.body.appendChild(resultBody);

    }



    function mod() {


        let numberOne = prompt("Enter number one:");

        let numberTwo = prompt("Enter number two:");

        modulus = Number(numberOne) % Number(numberTwo);

        let resultBody = document.createElement("p");

        resultBody.textContent = `${numberOne} % ${numberTwo} = ${modulus}`;

        document.body.appendChild(resultBody);

    }

</script>



<!--Head title of the task using head tag-->


    <title>Mod or Add</title>
</head>

<body>

    <!--Purpose of the task-->

    <h1>Calculate Add or Modulus</h1>
    <p>Press one or both of the buttons</p>


    <!--Declaring buttons in order to input values-->
    <div class="button">

        <input type="button" value="Click for adding" onclick="add()">


        <input type="button" value="Click for modulus" onclick="mod()">

        <p id="sum"></p>

    </div>







</body><!--Declaring script tag to perform functions from buttons above-->
</html>
