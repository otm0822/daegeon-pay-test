<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <script src="jquery-3.4.1.js"></script>

</head>
<body>
    <section class="login-form">
        <h1>Daegeon Pay</h1>
        <form action="">
            <div class ="int-area">
                <input type="text" name="id" id="id" autocomplete="off" required>
                <label for="id">USER NAME</label>
            <div>
            <div class ="int-area">
                <input type="password" name="pw" id="pw" autocomplete="off" required>
                <label for="PASSWORD">Password</label>
            <div>
            <div class="btn-area">
                <button id="btn"
                type="submit">LOGIN</button>
            </div>     
        </form>
        <div class="caption">
        <a href="#" onclick="location.href='google.com'">클릭</a>
    </section>

    <script>
        let id = $('#id')
        let pw = $('#pw')
        let btn = $('#btn')

        $(btn).on('click', function(){
            if($(id).val()==""){
                $(id).next('label').addClass('warning')
            }
            else if($(pw).val()==""){
                $(pw).next('label').addClass('warning')
                
            }
        });

    </script>
    
</body>
</html>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
