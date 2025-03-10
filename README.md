<!DOCTYPE html>
<html lang="kk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Shera TV</title>
<style>
body {
ont-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background: url('https://sun9-67.userapi.com/YbDsBRJPrYaPMECkr3zil7JVmwJd5SQO3kLIzA/vTFtKXL4MGA.jpg') no-repeat center center/cover;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;}
.container {
    background: rgba(0, 0, 0, 0.7);
    padding: 30px;
    border-radius: 15px;
    box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.3);
    text-align: center;}
h1 {
    margin-bottom: 20px;
    font-size: 32px;}
label {
    font-size: 20px;
    font-weight: bold;}
input {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: none;
    border-radius: 5px;
    font-size: 18px;}
.btn {
    display: inline-block;
    background: #ff6600;
    color: white;
    text-decoration: none;
    padding: 12px 20px;
    font-size: 18px;
    border-radius: 5px;
    cursor: pointer;
    transition: 0.3s;
    border: none;}
.btn:hover {background: #cc5500;}
</style>
</head>
<body>
<div class="container">
    <header>
        <h1>Shera TV 🧌</h1>
    </header>
<label for="email">Email</label><br>
<input type="text" id="email" name="email" required><br>

<label for="password">Password</label><br>
<input type="password" id="password" name="password" required><br>
        
<button class="btn" onclick="validateLogin()">Jiberu</button>
</div>
<script>
function validateLogin() {
    var email = document.getElementById('email').value;
    var password = document.getElementById('password').value;
            var validCredentials = {
                "xxan5604@gmail.com": "123456",
                "xan5604@gmail.com": "123456",
                "tt@gmail.com": "123456"
            };
            if (validCredentials[email] && validCredentials[email] === password) {
                window.location.href = "1 бет.html";
            } else {
                alert("Қате email немесе пароль⁉️🧐"); 
            }
        }
</script>
</body>
</html>
