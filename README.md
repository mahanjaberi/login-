# login-
my login web page
<!DOCTYPE html>
<html>
<head>
    <title>login</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        body {
            background-color: black;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .form-container {
            background: rgba(193, 166, 211, 0.1);
            padding: 50px;
            border-radius: 15px;
            box-shadow: 0 0 15px rgba(0, 255, 255, 0.4);
            width: 320px;
            text-align: center;
        }
        h2 {
            color: aqua;
            margin-bottom: 20px;
        }
        .input-box {
            position: relative;
            margin: 19px 0;
        }
        .input-box input {
            width: 100%;
            padding: 12px 15px;
            background: none;
            border: none;
            outline: none;
            color: beige;
            font-size: 18px;
            border-bottom: 2px solid rgba(255, 255, 255, 0.5);
            transition: 0.4s;
        }
        .input-box input:focus {
            border-color: beige;
            box-shadow: 0 5px 15px rgba(0, 255, 255, 0.3);
        }
        .input-box span {
            position: absolute;
            top: 50%;
            left: 15px;
            color: rgba(0, 255, 255, 0.5);
            font-size: 16px;
            pointer-events: none;
            transition: 0.4s;
            transform: translateY(-50%);
        }
        .input-box input:focus + span,
        .input-box input:not(:placeholder-shown) + span {
            top: 5px;
            font-size: 12px;
            color: azure;
        }
        .submit-btn {
            background: linear-gradient(90deg, #0ce442, #0f32e0);
            border: none;
            padding: 12px 30px;
            border-radius: 25px;
            color: #000;
            font-weight: bold;
            cursor: pointer;
            transition: 0.4s;
            margin-top: 10px;
        }
        .submit-btn:hover {
            background: linear-gradient(99deg, #00ff80, #00ffff);
            box-shadow: 0 5px 15px #00ffff80;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <h2>LOGIN</h2>
        <form>
            <div class="input-box">
                <input type="text" id="username" placeholder="" required>
                <span>username</span>
            </div>
            <div class="input-box">
                <input type="password" id="password" placeholder="" required>
                <span>password</span>
            </div>
            <button type="submit" class="submit-btn">submit</button>
        </form>
    </div>
</body>
</html>
