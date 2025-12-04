<!DOCTYPE html>
<html>
<head>
    <title>Mini Calculator</title>
    <meta charset="UTF-8">
    <style>
        body {
            font-family: Arial;
            text-align: center;
            margin-top: 60px;
            background-color: #f0f9ff;
        }

        h1 {
            color: #0f172a;
        }

        .box {
            background: white;
            padding: 20px;
            width: 300px;
            margin: auto;
            border-radius: 12px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        input {
            padding: 10px;
            width: 90%;
            margin-bottom: 10px;
            font-size: 16px;
            border-radius: 6px;
            border: 1px solid #94a3b8;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 8px;
            background-color: #10b981; /* green */
            color: white;
            transition: 0.3s;
        }

        button:hover {
            background-color: #059669; /* darker green */
        }

        #result {
            margin-top: 15px;
            font-size: 20px;
            color: #2563eb; /* blue */
        }
    </style>
</head>

<body>

    <h1>Mini Calculator</h1>

    <div class="box">
        <input type="number" id="num1" placeholder="Enter first number">
        <input type="number" id="num2" placeholder="Enter second number">

        <button onclick="add()">Add</button>

        <p id="result"></p>
    </div>

    <script>
        function add() {
            let n1 = Number(document.getElementById("num1").value);
            let n2 = Number(document.getElementById("num2").value);
            let sum = n1 + n2;

            document.getElementById("result").innerHTML = "Result: " + sum;
        }
    </script>

</body>
</html>
