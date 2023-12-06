# site-for-my-gf
<!DOCTYPE html>
<html>
<head>
    <title>Un Message pour Ma Copine</title>
    <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
    <div id="heartContainer" onclick="showHeart()">
        <div id="heart"></div>
        <p id="compliment" style="display:none;">Tu es incroyable !</p>
    </div>
    <script src="script.js"></script>
</body>
</html>
#heartContainer {
    text-align: center;
    margin-top: 50px;
}

#heart {
    width: 100px;
    height: 100px;
    background-color: red;
    position: relative;
    transform: rotate(45deg);
    display: none;
}

#heart:before, #heart:after {
    content: "";
    width: 100px;
    height: 100px;
    background-color: red;
    border-radius: 50%;
    position: absolute;
}

#heart:before {
    top: -50px;
    left: 0;
}

#heart:after {
    top: 0;
    left: 50px;
}

#compliment {
    font-size: 24px;
    margin-top: 20px;
}
function showHeart() {
    var heart = document.getElementById("heart");
    var compliment = document.getElementById("compliment");
    heart.style.display = "block";
    compliment.style.display = "block";
}
