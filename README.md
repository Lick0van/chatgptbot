<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мини-приложение Telegram</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }
        .container {
            text-align: center;
            background: white;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        button {
            padding: 10px 20px;
            margin: 10px;
            border: none;
            background-color: #4CAF50;
            color: white;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Добро пожаловать в мини-приложение!</h1>
        <button onclick="claimCoins()">Получить монеты</button>
        <button onclick="checkBalance()">Проверить баланс</button>
        <p id="message"></p>
    </div>
    <script>
        // Здесь будет ваша логика для взаимодействия с Telegram Bot API
        function claimCoins() {
            // Логика для получения монет
            document.getElementById('message').innerText = 'Вы получили 40 монет!';
        }

        function checkBalance() {
            // Логика для проверки баланса
            document.getElementById('message').innerText = 'У вас 100 монет.';
        }
    </script>
</body>
</html>
