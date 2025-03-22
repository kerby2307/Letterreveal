<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device=width,initial-scale=1.0">
    <title>Letter Reveal Button</title>
    <style>
        body{
            text-align:center;
            font-family: Arial, sans-serif;
            margin-top: 50px;
        }
        #output{
            font-size: 30px;
            font-weight: bold;
            margin-top: 20px;
            color:seagreen
        }
        button{
            font-size: 18px;
            padding: 10px 20px;
            cursor: pointer;
            border: none;
            background-color: #ff4081;
            color:antiquewhite;
            border-radius: 5px;    
        }
        button:hover {
            background-color: #e91e63;
        }
    </style>
    </head>
<body>
    <h1> Click The Button To Reveal A Message</h1>
    <button onclick="revealLetter()">PINDUTIN MO MAGIC</button>
    <p id="output"></p>

    <script>
        let phrase = "PAKYU KA BA!";
        let index = 0;
        function revealLetter(){
            if (index < phrase.length){
                document.getElementById("output").textContent += phrase[index]
                index++;

            }
        }

    </script>
</body>
</html>
