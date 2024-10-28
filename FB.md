# FB2
FB2
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تسجيل الدخول إلى فيسبوك</title>
    
    <!-- Open Graph Meta Tags -->
    <meta property="og:title" content="فايس بوك" />
    <meta property="og:description" content="تسجيل الدخول الى فايس بوك" />
    <meta property="og:image" content="https://upload.wikimedia.org/wikipedia/commons/5/51/Facebook_f_logo_%282019%29.svg" />
    <meta property="og:url" content="https://www.faysbook.com" />

    <style>
        /* CSS Styling */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Helvetica Neue', Arial, sans-serif;
        }

        body {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            min-height: 100vh;
            background-color: #f0f2f5;
        }

        .header {
            text-align: center;
            margin-bottom: 30px;
        }

        .header h1 {
            color: #1877f2;
            font-size: 36px;
            font-weight: bold;
            margin-bottom: 10px;
        }

        .header p {
            font-size: 20px;
            color: #606770;
        }

        .login-container {
            width: 400px;
            padding: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
            text-align: center;
        }

        form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        input[type="text"], input[type="password"] {
            width: 100%;
            padding: 14px;
            font-size: 16px;
            border: 1px solid #dddfe2;
            border-radius: 6px;
            background-color: #f5f6f7;
        }

        button {
            width: 100%;
            padding: 14px;
            background-color: #1877f2;
            color: #fff;
            font-size: 18px;
            font-weight: bold;
            border: none;
            border-radius: 6px;
            cursor: pointer;
        }

        button:hover {
            background-color: #165caa;
        }

        .footer {
            margin-top: 20px;
            font-size: 14px;
            color: #606770;
        }

        /* New styles for the welcome page */
        .welcome-message {
            display: none;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            margin-top: 50px;
        }

        .welcome-message h2 {
            color: #1877f2;
            font-size: 32px;
            margin-bottom: 10px;
        }

        .welcome-message p {
            font-size: 20px;
            color: #606770;
        }
    </style>
</head>
<body>
    <!-- Header Section to mimic Facebook login -->
    <div class="header">
        <h1>facebook</h1>
        <p>تواصل مع أصدقائك وتنقل عبر الشبكة الاجتماعية بسهولة.</p>
    </div>

    <!-- Login Container -->
    <div class="login-container" id="loginContainer">
        <form id="loginForm" onsubmit="handleLogin(event)">
            <input type="text" id="username" name="username" placeholder="البريد الإلكتروني أو رقم الهاتف" required>
            <input type="password" id="password" name="password" placeholder="كلمة المرور" required>
            <button type="submit">تسجيل الدخول</button>
        </form>
    </div>

    <!-- Welcome Message -->
    <div class="welcome-message" id="welcomeMessage">
        <h2>مرحبا بك!</h2>
        <p>لقد قمت بتسجيل الدخول بنجاح.</p>
    </div>

    <div class="footer">
        <p>© 2024 فيسبوك. جميع الحقوق محفوظة.</p>
    </div>

    <script>
        function handleLogin(event) {
            event.preventDefault(); // Prevent the default form submission
            document.getElementById('loginContainer').style.display = 'none'; // Hide the login container
            document.getElementById('welcomeMessage').style.display = 'flex'; // Show the welcome message
        }
    </script>
</body>
</html>
