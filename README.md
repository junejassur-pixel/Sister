<!DOCTYPE html>
<html>
<head>
    <title>Wizarding Birthday Surprise!</title>
    <style>
        body { background-color: #1a1a1a; display: flex; flex-direction: column; align-items: center; justify-content: center; height: 100vh; margin: 0; font-family: 'Georgia', serif; color: #eeba30; overflow: hidden; }
        .card { background: #740001; padding: 40px; border: 8px double #d3a625; border-radius: 15px; text-align: center; box-shadow: 0 0 30px rgba(0,0,0,0.5); position: relative; width: 350px; }
        h1 { font-size: 2.5em; text-shadow: 2px 2px #000; margin-bottom: 10px; }
        
        /* Better Cake Design */
        .cake { position: relative; width: 150px; height: 100px; background: #f3c623; border-radius: 10px 10px 0 0; margin: 50px auto 20px; box-shadow: inset 0 -10px rgba(0,0,0,0.1); }
        .cake::before { content: ""; position: absolute; top: -20px; left: 15px; width: 120px; height: 40px; background: #ae0001; border-radius: 50%; }
        .candle { position: absolute; top: -45px; left: 50%; transform: translateX(-50%); width: 8px; height: 30px; background: #fff; border-radius: 4px; }
        .flame { position: absolute; top: -15px; left: 50%; transform: translateX(-50%); width: 12px; height: 18px; background: orange; border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%; animation: flicker 0.1s infinite alternate; }
        @keyframes flicker { from { transform: translateX(-50%) scale(1); opacity: 0.8; } to { transform: translateX(-50%) scale(1.1); opacity: 1; } }

        /* Music Button */
        .magic-btn { background: #eeba30; color: #740001; border: none; padding: 15px 30px; font-size: 1.2em; font-weight: bold; border-radius: 50px; cursor: pointer; margin-top: 20px; transition: 0.3s; box-shadow: 0 5px #ae0001; }
        .magic-btn:active { transform: translateY(4px); box-shadow: 0 2px #ae0001; }
    </style>
</head>
<body>

    <div class="card">
        <h1>Happy Birthday!</h1>
        <p>A Very Magical Day to You, Muggle!</p>
        
        <div class="cake">
            <div class="candle"><div class="flame"></div></div>
        </div>

        <button class="magic-btn" onclick="playMusic()">⚡ Cast Music Spell</button>
    </div>

    <div id="music-container"></div>

    <script>
        function playMusic() {
            // This embeds the Harry Potter theme music link you provided
            document.getElementById('music-container').innerHTML = 
                '<iframe width="0" height="0" src="https://youtube.com" frameborder="0" allow="autoplay"></iframe>';
            alert("Accio Music! ⚡");
        }
    </script>

</body>
</html>
