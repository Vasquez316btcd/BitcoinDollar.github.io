    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tabbed Navigation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        .tab {
            overflow: hidden;
            background-color: #333;
        }
        .tab button {
            background-color: inherit;
            float: left;
            border: none;
            outline: none;
            cursor: pointer;
            padding: 14px 20px;
            color: white;
            font-size: 17px;
        }
        .tab button:hover {
            background-color: #575757;
        }
        .tab button.active {
            background-color: #04AA6D;
        }
        .tab-content {
            display: none;
            padding: 20px;
            border-top: none;
        }
        .tab-content.active {
            display: block;
        }
    </style>
</head>
<body>

    <div class="tab">
        <button class="tablinks active" onclick="openTab(event, 'home')">Home</button>
        <button class="tablinks" onclick="openTab(event, 'about')">About</button>
        <button class="tablinks" onclick="openTab(event, 'media')">Media</button>
        <button class="tablinks" onclick="openTab(event, 'creators')">Creators</button>
   
    </script>

</body>
</html>
