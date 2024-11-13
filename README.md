<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Page</title>
    <style>
        body {
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            font-family: 'Roboto', Arial, sans-serif;
            color: #555;
            background-color: #f5f5f5;
            flex-direction: column;
            text-align: center;
        }

        h1 {
            font-size: 2em;
            margin: 20px;
            color: #333;
        }

        /* Initial screen */
        .initial-screen {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            font-size: 1.2em;
        }

        button {
            padding: 10px 20px;
            font-size: 1em;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 4px;
            background-color: #4285F4;
            color: white;
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #357AE8;
        }

        /* Ready screen */
        .ready-screen {
            display: none;
            background-color: #ffffff;
            padding: 20px;
            border-radius: 10px;
            position: relative;
            z-index: 1;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .ready-screen h1 {
            font-size: 1.5em;
            margin-top: 20px;
        }

        .decorations {
            font-size: 2em;
            margin: 20px 0;
        }
    </style>
</head>
<body>

    <!-- Initial screen with prompt -->
    <div class="initial-screen">
        <p>Huuy mijidee yum asuuy</p>
        <button id="yesButton">Zaa</button>
        <button id="noButton">Ugui</button>
    </div>

    <!-- Ready screen -->
    <div class="ready-screen" id="readyScreen">
        <h1>~Nadtai uyrheej >-<.</h1>
        <div class="decorations">🌸❤️🌸❤️</div>
    </div>

    <script>
        // Add event listener to the "Yes" button
        document.getElementById("yesButton").addEventListener("click", function() {
            // Hide the initial screen and show the ready screen
            document.querySelector('.initial-screen').style.display = 'none';
            document.getElementById('readyScreen').style.display = 'block';
        });
    </script>

</body>
</html>
