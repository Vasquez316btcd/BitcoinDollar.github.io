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
    </div>

    <div id="home" class="tab-content active">
        <h2>Home</h2>
        <p>Welcome to the homepage.</p>
    </div>

    <div id="about" class="tab-content">
        <h2>About</h2>
        <p>Learn more about us.</p>
    </div>

    <div id="media" class="tab-content">
        <h2>Media</h2>
        <p>Explore our media gallery.</p>
    </div>

    <div id="creators" class="tab-content">
        <h2>Creators</h2>
        <p>Meet the creators behind this project.</p>
    </div>

    <script>
        function openTab(evt, tabName) {
            var i, tabcontent, tablinks;

            // Hide all tab contents
            tabcontent = document.getElementsByClassName("tab-content");
            for (i = 0; i < tabcontent.length; i++) {
                tabcontent[i].style.display = "none";
            }

            // Remove the "active" class from all tabs
            tablinks = document.getElementsByClassName("tablinks");
            for (i = 0; i < tablinks.length; i++) {
                tablinks[i].className = tablinks[i].className.replace(" active", "");
            }

            // Show the selected tab and mark the button as active
            document.getElementById(tabName).style.display = "block";
            evt.currentTarget.className += " active";
        }
    </script>

</body>
</html>
