<!DOCTYPE html>
<html>
<head>
<title>SCO ADS</title>
<script type="text/javascript">
    <!--
    if (screen.width <= 699) {
    document.location = "mobile.html";
}
</script>  
<meta name="viewport" content="width=device-width, initial-scale=1">
<link href='https://fonts.googleapis.com/css?family=Cinzel Decorative' rel='stylesheet'>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Tangerine">
<link href="https://fonts.googleapis.com/css2?family=Krona+One&display=swap" rel="stylesheet">
<link rel="stylesheet" href="cssweb/body.css">
<link rel="stylesheet" href="cssweb/header1.css" media="screen, print">
</head>
<body>
<!-- <div class="logo"><a href="#"><img src="#"></a></div> -->
<nav>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Tlgrm</a></li>
        <li><a href="#">Dscrd</a></li>
        <li><a href="#">About</a></li>


    </ul>

</nav>
<div id="sco" for="subject">SHIPPING CO.</div>
<div class="container1">
<form method="post" onsubmit="return submitUserForm();" action="send.php">
    <br/>
    <textarea input id="subject" name="msg" placeholder="Write something..." style="height:200px"></textarea>
    <div class="g-recaptcha" data-size="normal" data-sitekey="13a42369-3584-4f0e-b3c5-2df89f077d24" data-theme="dark" data-callback="verifyCaptcha"></div>
    <div id="g-recaptcha-error"></div>
    <input type="submit" name="submit" value="Submit" />
</form>
</div>
<!-- <script src='https://www.google.com/recaptcha/api.js'></script> -->
<script src="https://hcaptcha.com/1/api.js?hl=en-GB" async defer></script>
<script>
function submitUserForm() {
    var response = grecaptcha.getResponse();
    if(response.length == 0) {
        document.getElementById('g-recaptcha-error').innerHTML = '<span style="color:red;">This field is required.</span>';
        return false;
    }
    return true;
}
 
function verifyCaptcha() {
    document.getElementById('g-recaptcha-error').innerHTML = '';
}
</script>
</body>
</html>
