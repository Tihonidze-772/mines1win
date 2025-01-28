<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Choose Language</title>
<style>
    @font-face {
        font-family: 'Intro';
        src: url('intro.otf') format('opentype');
    }
    body {
        font-family: 'Intro', sans-serif;
        background-image: url('fon.jpg');
        background-size: cover;
        background-position: center;
        height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin: 0;
    }
    .buttons {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .button {
        background-color: orange;
        border: none;
        color: white;
        padding: 10px; /* was 20px */
        text-align: center;
        text-decoration: none;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 16px; /* was 32px */
        margin: 2px 7.5px; /* was 4px 15px */
        cursor: pointer;
        width: 100px; /* was 200px */
        height: 50px; /* was 100px */
        transition: all 0.3s ease;
        border-radius: 7.5px; /* was 15px */
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
        position: relative;
        overflow: hidden;
    }
    .button:before {
        content: "";
        position: absolute;
        top: 0;
        left: -37.5px; /* was -75px */
        width: 300%;
        height: 100%;
        background: rgba(255, 255, 255, 0.2);
        transform: skewX(-30deg);
        transition: left 0.7s ease;
    }
    .button:hover:before {
        left: 100%;
    }
    .button:hover {
        background-color: #e69500;
        box-shadow: 0 3px 6px rgba(0, 0, 0, 0.3);
        transform: translateY(-1px); /* was -2px */
    }
    h1 {
        color: white;
        margin-bottom: 20px; /* was 40px */
        font-size: 32px; /* was 64px */
        text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
    }
</style>
</head>
<body>
    <h1>Choose Language</h1>
    <div class="buttons">
        <a href="rus.html" class="button">RUS</a>
        <a href="en.html" class="button">ENG</a>
    </div>
</body>
</html>
