<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>White Paper Content</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <button onclick="showContent('h1')">Show H1</button>
        <button onclick="showContent('h2')">Show H2</button>
        <button onclick="showContent('h3')">Show H3</button>
        <button onclick="showContent('h4')">Show H4</button>
        <button onclick="showContent('h5')">Show H5</button>
        <button onclick="showContent('h6')">Show H6</button>

        <div id="content">
            <h1 class="content-section"><b>Creator H1 Header</b></h1>
            <h2 class="content-section"><b>H2 Header</b></h2>
            <h3 class="content-section"><b>H3 Header</b></h3>
            <h4 class="content-section"><b>H4 Hunter</b></h4>
            <h5 class="content-section"><b>H5 Header</b></h5>
            <h6 class="content-section"><b>H6 Header</b></h6>
        </div>
    </div>

    <script>
        function showContent(header) {
            document.querySelectorAll('.content-section').forEach(section => {
                section.style.display = 'none';
            });
            document.querySelector(header).style.display = 'block';
        }
    </script>
</body>
</html>
styles.css
body {
    font-family: Arial, sans-serif;
    text-align: center;
    margin: 50px;
    background-color: #f4f4f4;
}

.container {
    max-width: 600px;
    margin: auto;
    padding: 20px;
    background: #fff;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

button {
    margin: 5px;
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    background: #007bff;
    color: #fff;
    border-radius: 5px;
}

button:hover {
    background: #0056b3;
}

.content-section {
    display: none;
    margin-top: 20px;
    color: #333;
body {
    font-family: Arial, sans-serif;
    text-align: center;
    margin: 50px;
    background-color: #f4f4f4;
}

.container {
    max-width: 600px;
    margin: auto;
    padding: 20px;
    background: #fff;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

button {
    margin: 5px;
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    background: #007bff;
    color: #fff;
    border-radius: 5px;
}

button:hover {
    background: #0056b3;
}

.content-section {
    display: none;
    margin-top: 20px;
    color: #333;
}

