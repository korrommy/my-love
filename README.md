<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>valentine's day</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.2.3/css/bootstrap-grid.min.css"
        integrity="sha512-JQksK36WdRekVrvdxNyV3B0Q1huqbTkIQNbz1dlcFVgNynEMRl0F8OSqOGdVppLUDIvsOejhr/W5L3G/b3J+8w=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css"
        integrity="sha512-MV7K8+y+gLIBoVD59lQIYicR65iaqukzvf/nwasF0nqhPay5w/9lJmVM2hMDcnK1OnMGCdVK+iQrJ7lzPJQd1w=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.3/jquery.min.js"></script>
    <style>
        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 97vh;
        }

        .container svg {
            width: 50%;
            height: 50%;
        }
    </style>

    <!-- aa2 -->
    <style>
        * {
            margin: 0;
            padding: 0;
        }

        .body-letter {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #fae1dd;
        }

        .letter {
            position: relative;
            z-index: 1;
        }

        .valentines {
            position: relative;
            top: 50px;
            cursor: pointer;
            animation: up 3s linear infinite;
        }

        @keyframes up {

            0%,
            100% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(-30px);
            }
        }


        .envelope {
            position: relative;
            width: 300px;
            height: 200px;
            background-color: #f08080;
        }

        .envelope:before {
            background-color: #f08080;
            content: "";
            position: absolute;
            width: 212px;
            height: 212px;
            transform: rotate(45deg);
            top: -105px;
            left: 44px;
            border-radius: 30px 0 0 0;
        }

        .card {
            position: absolute;
            background-color: #eae2b7;
            width: 270px;
            height: 170px;
            top: 5px;
            left: 15px;
            box-shadow: -5px -5px 100px rgba(0, 0, 0, 0.4);
        }

        .card:before {
            content: "";
            position: absolute;
            border: 3px solid #003049;
            border-style: dotted;
            width: 240px;
            heighT: 140px;
            left: 12px;
            top: 12px;
        }

        .text {
            position: absolute;
            font-family: 'Brush Script MT', cursive;
            font-size: 28px;
            text-align: center;
            line-height: 25px;
            top: 19px;
            left: 85px;
            color: #003049;
        }

        .heart {
            background-color: #d62828;
            display: inline-block;
            height: 30px;
            margin: 0 10px;
            position: relative;
            top: 110px;
            left: 105px;
            transform: rotate(-45deg);
            width: 30px;
        }

        .heart:before,
        .heart:after {
            content: "";
            background-color: #d62828;
            border-radius: 50%;
            height: 30px;
            position: absolute;
            width: 30px;
        }

        .heart:before {
            top: -15px;
            left: 0;
        }

        .heart:after {
            left: 15px;
            top: 0;
        }

        .hearts {
            position: absolute;
            top: 0
        }

        .one,
        .two,
        .three,
        .four,
        .five {
            background-color: red;
            display: inline-block;
            height: 10px;
            margin: 0 10px;
            position: relative;
            transform: rotate(-45deg);
            width: 10px;
            top: 50px;
        }

        .one:before,
        .one:after,
        .two:before,
        .two:after,
        .three:before,
        .three:after,
        .four:before,
        .four:after,
        .five:before,
        .five:after {
            content: "";
            background-color: red;
            border-radius: 50%;
            height: 10px;
            position: absolute;
            width: 10px;
        }

        .one:before,
        .two:before,
        .three:before,
        .four:before,
        .five:before {
            top: -5px;
            left: 0;
        }

        .one:after,
        .two:after,
        .three:after,
        .four:after,
        .five:after {
            left: 5px;
            top: 0;
        }

        .one {
            left: 10px;
            animation: heart 1s ease-out infinite;
        }

        .two {
            left: 30px;
            animation: heart 2s ease-out infinite;
        }

        .three {
            left: 50px;
            animation: heart 1.5s ease-out infinite;
        }

        .four {
            left: 70px;
            animation: heart 2.3s ease-out infinite;
        }

        .five {
            left: 90px;
            animation: heart 1.7s ease-out infinite;
        }

        @keyframes heart {
            0% {
                transform: translateY(0) rotate(-45deg) scale(0.3);
                opacity: 1;
            }

            100% {
                transform: translateY(-150px) rotate(-45deg) scale(1.3);
                opacity: 0.5;
            }
        }

        .front {
            position: absolute;
            border-right: 180px solid #f4978e;
            border-top: 95px solid transparent;
            border-bottom: 100px solid transparent;
            left: 120px;
            top: 5px;
            width: 0;
            height: 0;
            z-index: 10;
        }

        .front:before {
            position: absolute;
            content: "";
            border-left: 300px solid #f8ad9d;
            border-top: 195px solid transparent;
            left: -120px;
            top: -95px;
            width: 0;
            height: 0;
        }

        .shadow {
            position: absolute;
            width: 330px;
            height: 25px;
            border-radius: 50%;
            background-color: rgba(0, 0, 0, 0.3);
            top: 265px;
            left: -15px;
            animation: scale 3s linear infinite;
            z-index: -1;
        }

        @keyframes scale {

            0%,
            100% {
                transform: scaleX(1);
            }

            50% {
                transform: scaleX(0.85);
            }
        }

        .hover-animation {
            animation: hover 1.75s ease-in-out infinite;
        }

        #castle {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #fae1dd;
        }

        .dustDef {
            position: absolute;
            background-color: white;
            border-radius: 100%;
            box-shadow: 0 0 3px 1px white;
            opacity: 0;
        }

        @keyframes hover {
            0% {
                margin-top: 60px;
            }

            50% {
                margin-top: 50px;
            }

            100% {
                margin-top: 60px;
            }
        }

        @keyframes glow {
            0% {
                box-shadow: 0 0 25px 0 #e8b2ca;
            }

            50% {
                box-shadow: 0 0 45px 0 #e8b2ca;
            }

            100% {
                box-shadow: 0 0 25px 0 #e8b2ca;
            }
        }

        @keyframes fall {
            5% {
                top: 209px;
                left: 105px;
                transform: rotate(55deg) scale(0.9, 0.95) skew(-18deg);
                opacity: 0.9;
            }

            30% {
                left: 90px;
            }

            55% {
                left: 130px;
            }

            60%,
            100% {
                top: 380px;
                transform: rotate(30deg) scale(0.9, 0.95) skew(-32deg);
                opacity: 0;
            }
        }

        @keyframes floatAnimate {
            0% {
                background-size: 105% 120%;
                background-position: 0 0;
                opacity: 0.7;
            }

            50% {
                background-size: 100% 100%;
                background-position: 0 0;
                opacity: 0.5;
            }

            100% {
                background-size: 105% 120%;
                background-position: 0 0;
                opacity: 0.7;
            }
        }
    </style>
    <style>
        svg {

            width: 80%;
            display: block;
            position: absolute;
            margin: auto;
            top: 0;
            bottom: 0;
            left: 0;
            right: 0;
            z-index: 1;
        }

        text {
            fill: #e6668a;
            font-family: consolas;
            font-size: 9px;
        }

        p {
            position: absolute;
            z-index: 2
        }

        label {
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
            opacity: .8
        }

        /* style letter */
        /* .box-content.active {
            opacity: 1;
            visibility: visible;
            transform: scale(1);
        }

        .box-content {
            position: fixed;
            width: 100%;
            height: 100%;
            z-index: 100000000000;
            top: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            background: rgba(0, 0, 0, 0.7);
            transform: scale(0.01);
            visibility: hidden;
            transition: 0.5s;
        }

        .fa-xmark {
            position: absolute;
            right: 5%;
            top: 5%;
            font-size: 40px;
            color: #fff;
            cursor: pointer;
        }

        .fa-xmark:hover {
            filter: drop-shadow(0 0 10px #fff);
        }

        .image-decorate {
            display: flex;
            width: 700px;
            z-index: 10;
            height: 100%;
        }

        .content1 {
            position: absolute;
            width: 700px;
            height: 500px;
            background-image: radial-gradient(circle farthest-corner at center, #f9edf3 10%, #ffd3ee 100%);
            border-radius: 10px 70px 10px 70px;
            box-shadow: 5px 5px 10px rgb(0, 0, 0);
            cursor: pointer;
        }

        .textLetter {
            width: 100%;
            flex-direction: column;
            justify-content: center;
            display: flex;
            align-items: center;
            user-select: none;
        }

        .textLetter h2 {
            font-size: 30px;
            font-family: 'Dancing Script', cursive;
        }

        .textLetter .contentLetter {
            font-size: 19px;
            text-align: center;
            padding: 0px 30px;
            margin-top: 10px;
            font-family: 'Dancing Script', cursive;
            position: initial;

        } */



        .letters{
    position: absolute;
    width: 65px;
    transition: 10s ease-in-out;
    cursor: pointer;
    z-index: 1000;
}
.letters img{
    width: 100%;
}
.wrapperLetterForm{
    position: absolute;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    z-index: 1000;
    background: rgba(0, 0, 0, 0.7);
    display: none;
}
.boxLetter{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}
.boxLetter .formLetter{
    position: relative;
    width: 600px;
    height: 350px;
    background-color: #FFEBEB;
    border-radius: 20px;
    z-index: 100;
    padding: 20px 15px;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}
.formLetter .wrapperLetter{
    position: relative;
    width: 100%;
    height: 100%;
    border: 2px dashed #FF6666;
    border-radius: inherit;
    display: flex;
}
.boxLetter .before{
    position: absolute;
    width: 600px;
    height: 350px;
    background: #fff;
    transform: rotate(-15deg);
    border-radius: 20px;
    z-index: 10;
}
.formLetter .heartLetter{
    position: absolute;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    background: #FFEBEB;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 10;
}
.heartLetter .heartLetterItem{
    position: relative;
    width: 10px;
    height: 10px;
    transform: rotate(45deg);
    background: #FF6666;
}
.heartLetter:first-child{
    right: 5px;
    top: 10px;
}
.heartLetter:nth-child(2){
    left: 5px;
    bottom: 10px;
}
.heartLetterItem::before, .heartLetterItem::after{
    position: absolute;
    content: '';
    width: 100%;
    height: 100%;
    border-radius: 50%;
    background: inherit;
}
.heartLetterItem::before{
    top: -50%;
}
.heartLetterItem::after{
    left: -50%;
}
.giftbox{
    position: relative;
    width: 40%;
    height: 100%;
}
.giftbox .img{
    position: absolute;
    width: 180px;
    bottom: -10px;
    left: 50px;
    z-index: 100;
}
.giftbox img{
    width: 100%;
}
.textLetter {
            width: 100%;
            flex-direction: column;
            justify-content: center;
            display: flex;
            align-items: center;
            user-select: none;
        }

        .textLetter h2 {
            font-size: 30px;
            font-family: 'Dancing Script', cursive;
        }

        .textLetter .contentLetter {
            font-size: 19px;
            text-align: center;
            padding: 0px 30px;
            margin-top: 10px;
            font-family: 'Dancing Script', cursive;
            position: initial;

        }
.fa-xmark{
    position: absolute;
    right: 20px;
    top: 20px;
    color: #fff;
    cursor: pointer;
    font-size: 25px;
}
.show{
    display: block;
}
.heartAnimation{
    position: absolute;
    width: 200px;
    bottom: 0;
}
.heartAnimation img{
    width: 100%;
}
.mewmew1, .mewmew2{
    position: absolute;
    width: 90px;
}
.mewmew1{
    bottom: 0;
    left: 0;
}
.mewmew2{
    bottom: 0;
    right: 0;
}
.mewmew1 img, .mewmew2 img{
    width: 100%;
}

    </style>
</head>

<body>

    <svg style="display: none;" id="theSvg" viewBox="-120 -30 240 180" enable-background="new 0 0 174 148"
        xml:space="preserve">
        <defs>
            <filter id="f" filterUnits="userSpaceOnUse" x="-120" y="-30" width="120%" height="120%">
                <feGaussianBlur in="SourceAlpha" stdDeviation="5" result="blur"></feGaussianBlur>
                <feOffset in="blur" dx="3" dy="5" result="shadow"></feOffset>
                <feFlood flood-color="rgba(3,0,0,1)" result="color" />
                <feComposite in="color" in2="shadow" operator="in" />
                <feComposite in="SourceGraphic" />
            </filter>
            <path id="shape" d="M0, 21.054 
       C0, 21.054 24.618, -15.165 60.750, 8.554 
       C93.249, 29.888 57.749, 96.888 0, 117.388
       C-57.749, 96.888  -93.249, 29.888 -60.750, 8.554
       C-24.618, -15.165  -0, 21.054 -0, 21.054z    
    " />
            <path id="partialPath" />

        </defs>

        <text dy="-2">
            <textPath style="font-family: fantasy;" xlink:href="#partialPath" startOffset="12">
                ????Happy Varentine's Day
                ????.........................................................................................................................................????From
                With Love 8/3!????
            </textPath>
        </text>

        <use id="useThePath" xlink:href="#partialPath" stroke="white" stroke-width=".5" stroke-opacity=".5" fill="none"
            style="display:none;" />
    </svg>

    <script>
        let rid = null; // request animation id
        const SVG_NS = "http://www.w3.org/2000/svg";
        const pathlength = shape.getTotalLength();

        let t = 0; // at the begining of the path
        let lengthAtT = pathlength * t;

        let d = shape.getAttribute("d");

        // 1. build the d array
        let n = d.match(/C/gi).length; // how many times

        let pos = 0; // the position, used to find the indexOf the nth C

        class subPath {
            constructor(d) {
                this.d = d;
                this.get_PointsRy();
                this.previous = subpaths.length > 0 ? subpaths[subpaths.length - 1] : null;
                this.measurePath();
                this.get_M_Point(); //lastPoint
                this.lastCubicBezier;
                this.get_lastCubicBezier();
            }

            get_PointsRy() {
                this.pointsRy = [];
                let temp = this.d.split(/[A-Z,a-z\s,]/).filter(v => v); // remove empty elements
                temp.map(item => {
                    this.pointsRy.push(parseFloat(item));
                }); //this.pointsRy numbers not strings
            }

            measurePath() {
                let path = document.createElementNS(SVG_NS, "path");
                path.setAttributeNS(null, "d", this.d);
                // no need to append it to the SVG
                // the lengths of every path in dry
                this.pathLength = path.getTotalLength();
            }

            get_M_Point() {
                if (this.previous) {
                    let p = this.previous.pointsRy;
                    let l = p.length;
                    this.M_point = [p[l - 2], p[l - 1]];
                } else {
                    let p = this.pointsRy;
                    this.M_point = [p[0], p[1]];
                }
            }

            get_lastCubicBezier() {
                let lastIndexOfC = this.d.lastIndexOf("C");
                let temp = this.d
                    .substring(lastIndexOfC + 1)
                    .split(/[\s,]/)
                    .filter(v => v);
                let _temp = [];
                temp.map(item => {
                    _temp.push(parseFloat(item));
                });
                this.lastCubicBezier = [this.M_point];
                for (let i = 0; i < _temp.length; i += 2) {
                    this.lastCubicBezier.push(_temp.slice(i, i + 2));
                }
            }
        }

        let subpaths = [];

        // create new subPaths
        for (let i = 0; i < n; i++) {
            // finds the of nth C in d
            let newpos = d.indexOf("C", pos + 1);
            if (i > 0) {
                // if it's not the first C
                let sPath = new subPath(d.substring(0, newpos));
                subpaths.push(sPath);
            }
            //change the value of the position pos
            pos = newpos;
        }
        // at the end add d to the subpaths array
        subpaths.push(new subPath(d));

        // 2. get the index of the bezierLengths where the point at t is
        let index;
        for (index = 0; index < subpaths.length; index++) {
            if (subpaths[index].pathLength >= lengthAtT) {
                break;
            }
        }

        function get_T(t, index) {
            let T;
            lengthAtT = pathlength * t;
            if (index > 0) {
                T =
                    (lengthAtT - subpaths[index].previous.pathLength) /
                    (subpaths[index].pathLength - subpaths[index].previous.pathLength);
            } else {
                T = lengthAtT / subpaths[index].pathLength;
            }
            //console.log(T)
            return T;
        }

        let T = get_T(t, index);

        let newPoints = getBezierPoints(T, subpaths[index].lastCubicBezier);

        drawCBezier(newPoints, partialPath, index);

        function getBezierPoints(t, points) {
            let helperPoints = [];

            // helper points 0,1,2
            for (let i = 1; i < 4; i++) {
                //points.length must be 4 !!!
                let p = lerp(points[i - 1], points[i], t);
                helperPoints.push(p);
            }

            // helper points 3,4
            helperPoints.push(lerp(helperPoints[0], helperPoints[1], t));
            helperPoints.push(lerp(helperPoints[1], helperPoints[2], t));

            // helper point 5 is where the first Bézier ends and where the second Bézier begins
            helperPoints.push(lerp(helperPoints[3], helperPoints[4], t));

            // points for the dynamic bézier
            let firstBezier = [
                points[0],
                helperPoints[0],
                helperPoints[3],
                helperPoints[5]
            ];
            //console.log(firstBezier)
            return firstBezier;
        }

        function lerp(A, B, t) {
            let ry = [
                (B[0] - A[0]) * t + A[0], //x
                (B[1] - A[1]) * t + A[1] //y
            ];
            return ry;
        }

        function drawCBezier(points, path, index) {
            let d;

            if (index > 0) {
                d = subpaths[index].previous.d;
            } else {
                d = `M${points[0][0]},${points[0][1]} C`;
            }

            // points.length == 4
            for (let i = 1; i < 4; i++) {
                d += ` ${points[i][0]},${points[i][1]} `;
            }
            //console.log(d)
            partialPath.setAttributeNS(null, "d", d);
        }
    </script>

    <div id="castle" style="display: none;">
        <div class="letter">
            <div class="valentines">
                <div class="envelope"></div>
                <div class="front"></div>
                <div class="card">
                    <div class="text">Happy</br> Varentine's</br> Day!</div>
                    <div class="heart"></div>
                </div>
                <div class="hearts">
                    <div class="one"></div>
                    <div class="two"></div>
                    <div class="three"></div>
                    <div class="four"></div>
                    <div class="five"></div>
                </div>
            </div>
            <div class="shadow"></div>
        </div>

    </div>


    <div class="container" id="rose-t">
        <svg viewBox="0 0 512 512">
            <path class="leafOne" d="M124.302,328.222c-2.466-2.901-5.036-5.334-7.648-7.212c-1.884-1.354-4.49-1.207-6.201,0.36
                                    c-32.608,29.866-18.892,84.017,24.01,94.752c2.251,0.563,4.612-0.548,5.624-2.636c0.407-0.841,0.781-1.732,1.138-2.648
                                    C111.438,394.378,103.302,355.204,124.302,328.222z" />
            <path class="stickLine"
                d="M337.625,212.314c2.37-3.44,1.501-8.149-1.939-10.519c-3.44-2.369-8.15-1.501-10.519,1.939
                                     c-19.493,28.304-43.492,60.076-72.147,92.853l-2.542-30.875c-0.343-4.163-4-7.261-8.158-6.917c-4.163,0.343-7.26,3.995-6.917,8.158
                                     l3.721,45.196C172.176,385.546,93.558,449.444,4.053,496.37c-3.699,1.94-5.127,6.512-3.187,10.211
                                     c1.352,2.579,3.983,4.054,6.705,4.054c1.183,0,2.385-0.279,3.505-0.867c63.84-33.47,124.784-76.962,181.511-129.479
                                     c5.891-2.031,32.15-10.225,68.671-8.819c4.156,0.167,7.689-3.09,7.85-7.266c0.161-4.174-3.092-7.689-7.267-7.849
                                     c-18.678-0.721-34.824,0.89-47.384,3.036C259.688,314.785,301.126,265.31,337.625,212.314z" />
            <path class="leafTwo" d="M329.58,413.715c30.055,1.827,57.188-13.413,71.993-37.343c1.738-2.81,1.253-6.495-1.142-8.771
                                   c-13.04-12.394-37.78-21.675-66.625-23.428s-54.527,4.464-68.972,15.187c-2.653,1.969-3.581,5.568-2.196,8.568
                                   C274.438,393.475,299.525,411.888,329.58,413.715z" />
            <path class="leafS1" d="M370.677,231.945c-8.984-2.411-17.479-7.138-24.516-14.205c-5.085-5.106-8.742-10.981-11.143-17.242
                                  c-6.645,0.902-13.554,0.516-20.475-1.491c-9.578-2.778-17.805-7.959-24.234-14.68c-12.216,1.01-22.611,4.593-28.859,9.642
                                  c-1.416,1.145-1.839,3.149-0.999,4.772c7.157,13.821,21.478,23.41,38.131,23.745c11.548,0.232,22.109-4.035,30.031-11.178
                                  c-2.461,10.379-1.13,21.692,4.621,31.709c8.293,14.445,23.583,22.401,39.142,22.039c1.826-0.042,3.382-1.376,3.705-3.168
                                  C377.509,253.982,375.658,243.144,370.677,231.945z" />
            <path class="rose1" d="M508.212,99.848c-2.666-4.581-27.324-44.843-71.558-48.206c-4.268-0.223-8.58-0.164-12.816,0.176
                                l-1.148,0.092l0.471,1.051c7.005,15.648,9.002,31.447,7.106,48.307l0.877,0.04c11.782,0.538,23.679,3.513,35.362,8.841l0.367,0.168
                                l0.355-0.188c10.841-5.728,22.445-6.783,35.477-3.225C506.927,108.058,510.397,103.599,508.212,99.848z M452.476,54.541c-4.96-1.457-10.233-2.474-15.823-2.899c-4.268-0.223-8.58-0.164-12.816,0.176
                                l-1.148,0.092l0.471,1.051c7.005,15.648,9.002,31.447,7.106,48.307l0.877,0.04c9.334,0.426,18.74,2.407,28.055,5.851
                                C461.04,88.852,458.784,71.19,452.476,54.541z" />

            <path class="rose2" d="M418.642,40.96c-24.19-37.169-71.346-39.455-76.643-39.593c-4.34-0.114-6.582,5.071-3.543,8.22
                                 c9.38,9.721,14.029,20.406,14.212,32.665l0.005,0.402l0.324,0.242c13.637,10.194,23.714,22.558,29.944,36.731
                                 c4.198,10.201,6.37,19.468,7.545,29.411l0.996-0.402c8.962-3.617,18.525-6.008,28.405-7.105c3.688-0.322,7.481-0.397,11.274-0.223
                                 l0.762,0.035C434.378,79.498,430.171,59.623,418.642,40.96z " />

            <path class="rose3" d="M343.8,146.676c13.018-17.726,29.06-30.524,47.682-38.039l0.576-0.232
                                 c-1.161-9.857-3.49-19.395-7.611-29.408c-20.694-47.084-74.317-58.577-80.363-59.731c-4.853-0.927-8.31,4.471-5.489,8.546
                                 c21.533,31.149,7.895,59.383-14.633,90.009l0.071,0.029c-16.953,26.497-7.863,61.237,18.513,76.865
                                 c3.932,2.33,8.219,4.207,12.806,5.537c6.757,1.959,13.752,2.469,20.787,1.514l1.017-0.138l-0.367-0.959
                                 C330.327,183.817,333.08,162.625,343.8,146.676z" />

            <path class="rose4"
                d="M510.726,141.7c-3.917-4.747-39.75-46.26-91.009-41.792c-21.664,2.405-52.653,12.308-77.277,45.856
                                 c-13.392,19.922-16.495,52.272,4.132,72.986c3.371,3.385,7.075,6.243,11.008,8.573c26.325,15.597,61.186,6.961,76.309-20.683
                                 l0.077,0.062c15.307-34.399,34.961-59.933,71.9-56.082C510.802,151.136,513.867,145.507,510.726,141.7z M370.903,162.627c27.904-38.017,75.307-57.751,121.144-38.743
                                 c-16.072-12.613-41.381-26.674-72.329-23.977c-21.664,2.405-52.653,12.308-77.277,45.856c-13.392,19.922-16.495,52.272,4.132,72.986
                                 c3.371,3.385,7.075,6.243,11.008,8.573c4.885,2.894,10.125,4.964,15.515,6.228C354.624,212.802,357.947,181.899,370.903,162.627z" />
        </svg>
        <p id="text-click" style=" display: none;   font-family: fantasy;
        color: indianred;
        font-size: 50px;
        top: 80%;">Click me now !</p>
    </div>

    <!-- <div class="box-content">
        <i class="fa-solid fa-xmark"></i>
        <div class="content1">
            <div class="image-decorate">
                <div class="textLetter">
                    <h2></h2>
                    <p class="contentLetter"></p>
                </div>
            </div>
        </div> -->


        <div class="wrapperLetterForm" style="display: none;">
            <div class="boxLetter">
                <i class="fa-solid fa-xmark"></i>
                <div class="formLetter">
                    <div class="heartLetter">
                        <div class="heartLetterItem"></div>
                    </div>
                    <div class="heartLetter">
                        <div class="heartLetterItem"></div>
                    </div>
                    
                    <div class="wrapperLetter">
                        <div class="giftbox">
                            <div class="img">
                                <img src="./image/giftbox.png" alt="">
                            </div>
                        </div>
                        <div class="textLetter">
                            <h2></h2>
                            <p class="contentLetter"></p>
                            <div class="heartAnimation">
                                <img src="./image/heartAnimation.gif" alt="">
                            </div>
                        </div>
                        <div class="mewmew1">
                            <img src="./image/mewmew.gif" alt="">
                        </div>
                        <div class="mewmew2">
                            <img src="./image/mewmew.gif" alt="">
                        </div>
                    </div>
                </div>
                <div class="before"></div>
            </div>
        </div>

    </div>



    <script src="https://cdnjs.cloudflare.com/ajax/libs/animejs/2.0.2/anime.min.js"></script>

    <!-- aa3 -->
    <script>

        (() => {
            setTimeout(() => {
                document.querySelector("#text-click").style.display = "inherit";
            }, 4000);
            document.querySelector("#rose-t").onclick = function () {
                document.querySelector("#rose-t").style.display = "none";
                document.querySelector("#castle").style.display = "flex";
                document.querySelector("#theSvg").style.display = "inherit"

                rid = window.requestAnimationFrame(Typing);
                function Typing() {
                    rid = window.requestAnimationFrame(Typing);
                    if (t >= 1) {
                        window.cancelAnimationFrame(rid);
                        rid = null;
                    } else {
                        t += 0.0025;
                    }

                    lengthAtT = pathlength * t;
                    for (index = 0; index < subpaths.length; index++) {
                        if (subpaths[index].pathLength >= lengthAtT) {
                            break;
                        }
                    }
                    T = get_T(t, index);
                    newPoints = getBezierPoints(T, subpaths[index].lastCubicBezier);
                    drawCBezier(newPoints, partialPath, index);
                }
            }
            const head = document.getElementsByTagName('head')[0];
            let animationId = 1;

            function CreateMagicDust(x1, x2, y1, y2, sizeRatio, fallingTime, animationDelay, node = 'main') {
                let dust = document.createElement('span');
                let animation = document.createElement('style');
                animation.innerHTML = '\
      @keyframes blink' + animationId + '{\
          0% {\
              top: ' + y1 + 'px;\
              left: ' + x1 + 'px;\
              width: ' + 2 * sizeRatio + 'px;\
              height: ' + 2 * sizeRatio + 'px;\
              opacity: .4\
          }\
          20% {\
              width: ' + 4 * sizeRatio + 'px;\
              height: ' + 4 * sizeRatio + 'px;\
              opacity: .8\
          }\
          35% {\
              width: ' + 2 * sizeRatio + 'px;\
              height: ' + 2 * sizeRatio + 'px;\
              opacity: .5\
          }\
          55% {\
              width: ' + 3 * sizeRatio + 'px;\
              height: ' + 3 * sizeRatio + 'px;\
              opacity: .7\
          }\
          80% {\
              width: ' + sizeRatio + 'px;\
              height: ' + sizeRatio + 'px;\
              opacity: .3\
          }\
          100% {\
              top: ' + y2 + 'px;\
              left: ' + x2 + 'px;\
              width: ' + 0 + 'px;\
              height: ' + 0 + 'px;\
              opacity: .1\
          }}';
                head.appendChild(animation);
                dust.classList.add('dustDef');
                dust.setAttribute('style', `animation: blink${animationId++} ${fallingTime}s cubic-bezier(.71, .11, .68, .83) infinite ${animationDelay}s`);
                document.getElementById(node).appendChild(dust);
            }

            // yes, I'm doing it manually to get the effect I want.. can be easily changed to render randomly
            [[130, 132, 150, 152, .15, 2.5, .1, 'sub'],
            [65, 63, 300, 299, .5, 2, .2, 'sub'],
            [70, 70, 150, 150, .45, 2, .5],
            [75, 78, 160, 170, .6, 2, 1],
            [80, 82, 160, 180, .6, 1, .4],
            [85, 100, 160, 170, .5, 2, .5],
            [125, 110, 170, 180, .25, 3, 1.5],
            [90, 90, 115, 115, .4, 2, 2],
            [93, 95, 200, 200, .4, 3, 1.5],
            [100, 100, 145, 155, .45, 1, .5],
            [100, 90, 170, 230, .35, 2, .75],
            [100, 102, 115, 112, .35, 3, .25],
            [100, 95, 170, 200, .55, 1.5, .75],
            [100, 97, 150, 190, .7, 2, 1.5],
            [105, 100, 160, 180, .5, 1.5, .725],
            [125, 125, 180, 190, .25, 1, .725],
            [130, 130, 135, 135, .45, 3, 1.5],
            [135, 132, 170, 190, .25, 2.5, .75],
            [135, 132, 320, 315, .2, 5, .3, 'sub']
            ].forEach((o) => CreateMagicDust(...o));

        })();
    </script>

    <script>
        // .textLetter text h2
        let indexText = 0;
        let textLetter = document.querySelector('.textLetter h2');
        const textLetterH2 = "ให้เนยเท่านั้น";
        let timoutTextLetter;

        function textCharLetter() {
            if (indexText < textLetterH2.length) {
                textLetter.textContent += textLetterH2[indexText];
                indexText++;
                setTimeout(indexText, 100);
            }
            else {
                clearInterval(timoutTextLetter);
                setTimeout(() => {
                    funcTimeoutLetterContent()
                }, 500)
            }
        }
        function funcTimeoutLetter() {
            indexText = 0; // Reset indexText
            textLetter.textContent = ''; // Xóa nội dung hiện tại của textLetter
            clearInterval(timoutTextLetter);
            timoutTextLetter = setInterval(() => {
                textCharLetter();
            }, 200)
        }

        // chữ của thư bạn muốn gửi
        let indexTextContent = 0;
        let textLetterContent = document.querySelector('.contentLetter');
        const textLetterP = "สุขสันต์วันวาเลนไทน์นะ????";
        let timoutTextLetterContent;
        function textCharLetterContent() {
            if (indexTextContent < textLetterP.length) {
                textLetterContent.textContent += textLetterP[indexTextContent];
                indexTextContent++;
                setTimeout(indexTextContent, 1);
            }
            else {
                clearInterval(timoutTextLetterContent)

            }
        }
        function funcTimeoutLetterContent() {
            indexTextContent = 0; // Reset indexTextContent
            textLetterContent.textContent = ''; // Xóa nội dung hiện tại của textLetter
            clearInterval(timoutTextLetterContent);
            timoutTextLetterContent = setInterval(() => {
                textCharLetterContent();
            }, 100)
        }
        $(document).ready(function () {
            $('.valentines').mouseenter(function () {
                $('.card').stop().animate({
                    top: '-90px'
                }, 'slow');
            }).mouseleave(function () {
                $('.card').stop().animate({
                    top: 0
                }, 'slow');
            });

            $('.card').click(function () {
                $('.box-content').addClass('active');
                $(".wrapperLetterForm").fadeIn()
                funcTimeoutLetter();
            });

            $('.fa-xmark').click(function () {
                $('.wrapperLetterForm').css('display','none');
            });
        });
        var leafOne = document.querySelector('.leafOne');
        var stickLine = document.querySelector('.stickLine');
        var leafTwo = document.querySelector('.leafTwo');
        var leafS1 = document.querySelector('.leafS1');
        var rose1 = document.querySelector('.rose1');
        var rose2 = document.querySelector('.rose2');
        var rose3 = document.querySelector('.rose3');
        var rose4 = document.querySelector('.rose4');

        var lineDrawing = anime({
            targets: [leafOne, stickLine, leafTwo, leafS1, rose1, rose2, rose3, rose4],
            strokeDashoffset: [anime.setDashoffset, 0],
            easing: 'easeInOutCubic',
            duration: 4000,
            begin: function (anim) {
                //Leaf One
                leafOne.setAttribute("stroke", "black");
                leafOne.setAttribute("fill", "none");
                // Leaf Two
                leafTwo.setAttribute("stroke", "black");
                leafTwo.setAttribute("fill", "none");
                //Stick
                stickLine.setAttribute("stroke", "black");
                stickLine.setAttribute("fill", "none");
                // Leaf S1
                leafS1.setAttribute("stroke", "black");
                leafS1.setAttribute("fill", "none");
                //Rose One
                rose1.setAttribute("stroke", "black");
                rose1.setAttribute("fill", "none");
                //Rose Two
                rose2.setAttribute("stroke", "black");
                rose2.setAttribute("fill", "none");
                //Rose Three
                rose3.setAttribute("stroke", "black");
                rose3.setAttribute("fill", "none");
                //Rose Three
                rose4.setAttribute("stroke", "black");
                rose4.setAttribute("fill", "none");
            },
            complete: function (anim) {
                //Leaf One
                leafOne.setAttribute("fill", "#9CDD05");
                leafOne.setAttribute("stroke", "none");
                //Leaf Two 
                leafTwo.setAttribute("fill", "#9CDD05");
                leafTwo.setAttribute("stroke", "none");
                //Stick
                stickLine.setAttribute("fill", "#83AA2E");
                stickLine.setAttribute("stroke", "none");
                // Leaf S1
                leafS1.setAttribute("fill", "#9CDD05");
                leafS1.setAttribute("stroke", "none");
                // Rose 1
                rose1.setAttribute("fill", "#F37D79");
                rose1.setAttribute("stroke", "none");
                // Rose 2
                rose2.setAttribute("fill", "#D86666");
                rose2.setAttribute("stroke", "none");
                // Rose 3
                rose3.setAttribute("fill", "#F37D79");
                rose3.setAttribute("stroke", "none");
                // Rose 3
                rose4.setAttribute("fill", "#D86666");
                rose4.setAttribute("stroke", "none");
            },
            autoplay: true,
        });

    </script>
</body>

</html>
