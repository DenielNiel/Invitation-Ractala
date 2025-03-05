<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Invitation</title>
    <style>
        @keyframes popup {
            0% { transform: scale(0.5); opacity: 0; }
            100% { transform: scale(1); opacity: 1; }
        }
        body {
            background: url('https://imgur.com/VbHiYb2.jpg') no-repeat center center fixed;
            background-size: cover;
            font-family: Arial, sans-serif;
            text-align: center;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            flex-direction: column;
        }
        .invitation {
            width: 90%; 
            max-width: 300px;
            background: white;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            text-align: center;
        }
        h1 {
            color: #d63384;
            font-size: 22px;
            margin-bottom: 8px;
            font-weight: bold;
        }
        p {
            font-size: 16px;
            color: #222;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div id="tapMessage" style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); font-size: 24px; font-weight: bold; cursor: pointer; background: rgba(255, 255, 255, 0.8); padding: 15px 25px; border-radius: 10px; box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);">Pencet sini dongg</div>
    
    <div class="container" id="invitationContainer" style="display: none;">
        <div class="invitation" style="animation: popup 0.5s ease-out;">
            <img src="https://imgur.com/L9nwvsE.jpg" alt="Invitation Image" style="width: 100%; border-radius: 10px; margin-bottom: 10px;">
            <h1>You Are Invited</h1>
            <p>Join us for a special dinner<br>with RACTALA!<br><br><strong>Date :</strong> 8 - 3 - 2025<br><strong>Time :</strong> 3.30PM<br><strong>Location :</strong> River side</p>
        </div>
    </div>
    <script>
        document.getElementById("tapMessage").addEventListener("click", function() {
            this.style.display = "none";
            document.getElementById("invitationContainer").style.display = "flex";
            document.getElementById("invitationContainer").style.animation = "popup 0.5s ease-out";
        });
    </script>
</body>
</html>
