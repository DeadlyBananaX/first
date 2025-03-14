# first
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    body{
        background-image: url('C:/Users/Public/Documents/marble.jpg');
        background-position: center;
        background-size: cover;
        background-repeat: repeat;
    }
    .container{
        flex-wrap: wrap;
        background-color: white;
        height: 400px;
        width: 600px;
        margin:auto;
        margin-top: 10%;
        border-radius: 10px;
        text-align: center;
        padding: 20px;
    }
    input{
        width: 80%;
        padding: 10px;
        margin: 10px;
        border: 1px solid rgb(155, 155, 155);
        border-radius: 10px;
    }
    button{
        width: 83%;
        padding: 10px;
        margin: 10px;
        border: none;
        border-radius: 10px;
        background: rgb(24, 24, 24);
        color: white;
        cursor: pointer;
    }
</style>
<body>
    <script>
        function onClick(){
            var email = document.getElementsByClassName("Email")[0].value;
            if (email == "") {
                document.getElementsByClassName("error1")[0].style.display = "inline-block";
            }
            else{
                document.getElementsByClassName("error1")[0].style.display = "none";
            }
        }
    </script>
    <div class="container">
        <h2>Log in</h2>
        <input type="email" placeholder="Email" class="Email">
        <input type="password" placeholder="password">
        <button onclick="onClick()">Изпащане</button>
        <br>
        <a href="C:\Users\PC101_8\Documents\РП12В\marble\Registration.html">Register</a>
        <br>
        <p class="error1" style="display: none; color: red;">*Invalid Email</p>
    </div>
</body>
</html>
