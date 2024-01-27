<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PLEXILE ARCADE PROXY</title> 
    <link rel="icon" type="image/png" href="https://cdn.glitch.global/5c2cb934-0c5a-4e22-9abd-1591c7cf6a9c/6e5e1dcc-f1f3-492d-a396-f3d7077ee68f.image-fotor-bg-remover-20230806125936%20(1).png?v=1691387992370">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <style>
        body {
            background: url(https://cdn.glitch.global/595c0b59-ffda-42dc-be07-bf0564511e92/6fa06a64-56e3-41f8-9777-9bcdf149b03c.image.png?v=1697314046228);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
        }
        h1 {
            font-size: 2em;
            margin-bottom: -3px;
        }
        .search-container {
            background: #27292e;
            display: flex;
            flex-direction: row;
            border: 2px solid #b03232;
            border-radius: 100px;
            padding: 1px;
            height: 45px;
            width: 600px;
            align-items: center; /* Center vertically */
        }
        .search-container input {
            background: #27292e;
            border: none;
            width: 100%;
            padding: 10px;
            outline: none;
            border-radius: 25px;
            font-size: 15px;
            font-weight: bold;
            text-align: center; /* Center horizontally */
        }
        .search-container button {
            border: none;
            background: transparent;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <img src="https://cdn.glitch.global/8533ca4b-6fa9-468c-a0bb-b90172e91dcc/04d0f9c2-4d9c-4db7-b356-751b458fdf3b.image.png?v=1691895722806">
    <link rel="stylesheet" href="/oldcss.css" />
    <div id="haha"></div>

    <div class="search-container">
        <input type="text" placeholder="Enter URL & Search The Web Freely..." maxlength="50" onkeypress="handleKeyPress(event)">
        <div class="search-icon">
            <script>
                function getSiteUrl() {
                    const siteUrl = window.location.href;
                    alert('Site URL: ' + siteUrl);
                }

                function handleKeyPress(event) {
                    // Check if the pressed key is Enter (key code 13)
                    if (event.key === 'Enter') {
                        getSite();
                    }
                }
            </script>
        </div>
    </div>

    <script>
        var haha = document.getElementById("haha");

        function lmao() {
            var lol = ['ㅤ'];

            var hehe = Math.floor(Math.random() * lol.length);
            haha.textContent = lol[hehe];
        }

        lmao()

        function getSite() {
            let inputValue = document.querySelector('input').value;

            if (!inputValue.startsWith('http://') && !inputValue.startsWith('https://')) {
                inputValue = 'http://' + inputValue;
            }

            const encodedValue = btoa(inputValue);
            window.location.href = "/web/_" + encodedValue + '_/';
        }
    </script>
</body>
</html>




        <!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/ioicons@1.0.4/dist/css/ioicons.min.css">
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-color: #16181C; /* Adjusted background color */
/* All text is black */
        }

        .header {
               background-color: #12161D; /* Change the color of the rectangle box here */
            color: #fff; /* Text color inside the rectangle box is white */
            text-align: center;
            padding: 15px 0;
            position: fixed;
            bottom: 10px;
            width: 98%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            border-radius: 25px;
        }

        .header-icons {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-start; /* Align icons to the left */
            margin-left: 10px; /* Add some margin for better spacing */
        }

        .header-icons i {
            font-size: 40px; /* Adjust icon size as needed */
            margin-bottom: 10px; /* Spacing between icons */
            cursor: pointer;
            transition: transform 0.2s;
        }

        .header-icons i:hover {
            transform: rotate(360deg);
        }

        #plexile-arcade {
            font-size: 28px; /* Made PLEXILE ARCADE text a bit longer */
            font-weight: bold;
            color: #b03232; /* Color of PLEXILE ARCADE text */
        }

        #copyright {
            font-size: 14px;
            margin-top: 10px;
            font-weight: bold; /* Increased font weight */
            color: #b03232; /* Color of C Copyright PLEXILE ARCADE text */
            cursor: pointer;
            transition: color 0.2s, transform 0.2s;
        }

        #copyright:hover {
            animation: shake 0.5s;
        }

        @keyframes shake {
            0% { transform: translateX(0); }
            25% { transform: translateX(-5px); }
            50% { transform: translateX(5px); }
            75% { transform: translateX(-5px); }
            100% { transform: translateX(5px); }
        }
    </style>
</head>

<body>
    <div class="header">
        <div class="header-icons">
            <i class="io io-logo-youtube"></i>
            <i class="io io-logo-discord"></i>
        </div>
        <div id="plexile-arcade">PLEXILE ARCADE</div>
        <div id="copyright" onclick="openCreditsURL()">© PLEXILE ARCADE 2024</div>
    </div>

    <script>
        function openCreditsURL() {
            // Replace 'your_credits_url' with the actual URL you want to link to
            window.location.href = '/';
        }
    </script>
</body>

</html>
