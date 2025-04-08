<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Для Сони</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #f0f0f0;
            overflow: hidden;
            position: relative;
        }

        .heart {
            position: absolute;
            width: 100px;
            height: 100px;
            background-color: red;
            transform: rotate(-45deg);
            animation: heartbeat 1.5s infinite;
        }

        .heart::before,
        .heart::after {
            content: '';
            position: absolute;
            width: 100px;
            height: 100px;
            background-color: red;
            border-radius: 50%;
        }

        .heart::before {
            top: -50px;
            left: 0;
        }

        .heart::after {
            left: 50px;
            top: 0;
        }

        @keyframes heartbeat {
            0%, 20%, 50%, 80%, 100% {
                transform: scale(1);
            }
            10% {
                transform: scale(1.1);
            }
            30% {
                transform: scale(0.9);
            }
        }

        .content {
            position: relative;
            z-index: 1;
            text-align: center;
            font-family: Arial, sans-serif;
            color: #333;
            padding: 20px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        audio {
            display: none;
        }
    </style>
</head>
<body>
    <div class="heart"></div>
    <div class="content">
        <h1>Привет, Соня!</h1>
        <p>Я хочу, чтобы ты знала, как сильно я тебя люблю. Ты — моё солнышко, которое освещает даже самые серые дни. Каждый миг, проведённый с тобой, наполняет мою жизнь радостью и счастьем. 🌞</p>
        <p>Несмотря на расстояние между нами, ты всегда в моём сердце. Я чувствую твою поддержку и тепло, даже когда мы далеко друг от друга. Ты — моя вдохновительница, и я благодарен судьбе за то, что ты есть в моей жизни. 💖</p>
        <p>Каждый день я мечтаю о том моменте, когда мы снова будем вместе, и смогу обнять тебя крепко-крепко. Ты — моя радость, моя муза, и я хочу, чтобы ты всегда знала, как ты важна для меня. 💕</p>
        <p>Пусть каждый твой день будет наполнен счастьем, как ты наполняешь мою жизнь. Я жду не дождусь, когда смогу снова увидеть твою улыбку! 😘</p>
        <audio controls autoplay loop>
            <source src="/storage/emulated/0/Download/Макс Корж - Пьяный Дождь.mp3" type="audio/mpeg">
            Ваш браузер не поддерживает аудио.
        </audio>
    </div>
</body>
</html>
