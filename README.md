# MyFirstRep
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>173.3d立方体</title>
    <style>
        .box{
            width:400px;
            height:400px;
            margin:0px auto;
            position: relative;
            transform-style: preserve-3d;
            perspective: 900px;
            transform: rotateY(30deg) rotateX(30deg);
            animation: run 8s linear infinite;
        }
        @keyframes run{
            0%{
                transform: rotateY(30deg) rotateX(30deg) rotateZ(30deg);
            }
            25%{
                transform: rotateY(120deg) rotateX(120deg) rotateZ(120deg);
        }50%{
                transform: rotateY(240deg) rotateX(240deg) rotateZ(240deg);
            }75%{
                transform: rotateY(360deg) rotateX(360deg) rotateZ(360deg)
            }
            100%{
                transform: rotateY(30deg) rotateX(30deg) rotateZ(30deg);
            }
        }
        .box div{
            width:100px;
            height:100px;
            position: absolute;
            top:calc(50% - 50px);
            left:calc(50% - 50px);
            line-height: 100px;
            text-align: center;
            font-size:40px;
            opacity: 0.8;
    
        }
        .box div:nth-child(1){
            background-color: gray;
            transform: translateZ(50px);
        }
        .box div:nth-child(2){
            background-color: cadetblue;
            transform: translateX(-50px) rotateY(-90deg);
        }
        .box div:nth-child(3){
            background-color: yellow;
            transform: translateY(-50px) rotateX(90deg);
        }
        .box div:nth-child(4){
            background-color: purple;
            transform: translateY(50px) rotateX(-90deg);
        }
        .box div:nth-child(5){
            background-color:green;
            transform: translateX(50px) rotateY(90deg);
        }
        .box div:nth-child(6){
            background-color:darkblue;
            transform: translateZ(-50px) rotateY(180deg);
        }
    </style>
</head>
<body>
    <div class="box">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
        <div>5</div>
        <div>6</div>
    </div>
</body>
</html>
