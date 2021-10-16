# heart-github
<!DOCTYPE html>
<head>
    <title>heart.com</title>
</head>
<body>
    <style>
        .heart{
            position: absolute;
            margin: auto;
            top: 0px;
            right: 0px;
            bottom: 0px;
            left: 0px;
            height: 50px;
            width: 50px;
            background-color: red;
            transform: rotate(-45deg);
            animation-name: beat;
            animation-duration: 1s;
            animation-iteration-count: infinite;
        }
        .heart::after{
            content: "";
            position: absolute;
            top: -25px;
            height: 50px;
            width: 50px;
            background-color: red;
            border-radius: 50%;
        }
        .heart::before{
            content: "";
            background-color:red;
            height: 50px;
            width: 50px;
            position: absolute;
            left: 25px;
            border-radius: 50%;
        }
        .back {
            position: fixed;
            padding: 0;
            margin: 0;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: white;
            animation-name: backdiv;
            animation-duration: 1s;
            animation-iteration-count: infinite;
        }

        @keyframes backdiv {
            50% {
            background: #ffe6f2;
            }
        }

        @keyframes beat {
            0% {
            transform: scale(1) rotate(-45deg);
            }
            50% {
            transform: scale(0.6) rotate(-45deg);
            }
        }
    </style>
    <div class="back"></div>
    <div class="heart"></div>
</body>
