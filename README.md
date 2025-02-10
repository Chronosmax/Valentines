<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: pink;
        }
        h1 {
            margin-top: 50px;
            color: red;
        }
        .buttons {
            margin-top: 20px;
            position: relative;
        }
        button {
            font-size: 20px;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            transition: 0.3s;
        }
        #yes {
            background-color: red;
            color: white;
        }
        #no {
            background-color: white;
            color: red;
            position: absolute;
        }
    </style>
</head>
<body>

    <h1>Will You Be My Valentine? ❤️</h1>
    
    <div class="buttons">
        <button id="yes" onclick="alert('Yay! 💖')">Yes</button>
        <button id="no" onmouseover="moveButton()">No</button>
    </div>

    <script>
        function moveButton() {
            let x = Math.random() * window.innerWidth - 100;
            let y = Math.random() * window.innerHeight - 50;
            document.getElementById("no").style.left = x + "px";
            document.getElementById("no").style.top = y + "px";
        }
    </script>

</body>
</html
