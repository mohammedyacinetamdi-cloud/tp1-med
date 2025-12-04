[index.html](https://github.com/user-attachments/files/23942096/index.html)
<!DOCTYPE html>
<html>
<head>
    <title>Simple App</title>
    <meta charset="UTF-8">
    <style>
        body {
            font-family: Arial;
            text-align: center;
            margin-top: 80px;
            background: #f1f5f9; /* light background */
        }

        h1 {
            color: #1e3a8a; /* dark blue */
        }

        button {
            padding: 12px 25px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 8px;
            background-color: #2563eb; /* blue */
            color: white;
            transition: 0.3s;
        }

        button:hover {
            background-color: #1e40af; /* darker blue */
        }

        #message {
            margin-top: 20px;
            font-size: 18px;
            color: #16a34a; /* green */
        }
    </style>
</head>
<body>

    <h1>Welcome to My Simple App</h1>

    <button onclick="showMessage()">Click Me</button>

    <p id="message"></p>

    <script>
        function showMessage() {
            document.getElementById("message").innerHTML = "Button clicked!";
        }
    </script>

</body>
</html>
