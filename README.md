<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Cash Prize</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 500px;
            margin: auto;
            background: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            border-radius: 5px;
        }
        .title {
            color: green;
            font-size: 24px;
            font-weight: bold;
        }
        .prize {
            color: #ff9800;
            font-size: 32px;
            font-weight: bold;
        }
        .email-input {
            margin: 20px 0;
        }
        input[type="email"] {
            padding: 10px;
            width: 100%;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .btn {
            background-color: #28a745;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        .btn:hover {
            background-color: #218838;
        }
        .footer {
            margin-top: 20px;
            font-size: 12px;
            color: #666;
        }
    </style>
</head>
<body>
    <div class="container">
        <p class="title">FREE CASH PRIZE!</p>
        <p>No Purchase Necessary</p>
        <p class="prize">WIN A $500.00 CASH PRIZE</p>
        <p>Today's entry will expire in <span id="timer">11:45:26</span></p>
        <form class="email-input" action="https://smrturl.co/a/s0ac79153fc/3706?s1=jony" method="GET">
            <input type="email" name="email" placeholder="Enter Email Address" required>
            <button type="submit" class="btn">Continue</button>
        </form>
        <div class="footer">
            <p>Limited To One Per Household</p>
        </div>
    </div>
    <script>
        // Countdown Timer Script
        function startTimer(duration, display) {
            let timer = duration, hours, minutes, seconds;
            setInterval(function () {
                hours = Math.floor(timer / 3600);
                minutes = Math.floor((timer % 3600) / 60);
                seconds = timer % 60;

                hours = hours < 10 ? "0" + hours : hours;
                minutes = minutes < 10 ? "0" + minutes : minutes;
                seconds = seconds < 10 ? "0" + seconds : seconds;

                display.textContent = hours + ":" + minutes + ":" + seconds;

                if (--timer < 0) {
                    timer = duration;
                }
            }, 1000);
        }

        window.onload = function () {
            const display = document.querySelector('#timer');
            const timeLimit = 11 * 3600 + 45 * 60 + 26; // 11:45:26 in seconds
            startTimer(timeLimit, display);
        };
    </script>
</body>
</html>
