<!DOCTYPE html>
<html>
<head>
    <title>Rem - Anime Character</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-image: url("https://wallpapercave.com/wp/wp3923445.png");
            background-position: center;
            background-size: cover;
            background-repeat: no-repeat;
        }
        .no-background {
            background-image: none !important;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
            align-items: center;
            visibility: hidden;
        }
        h1 {
            margin: 0 0 20px;
            font-size: 36px;
            font-weight: normal;
            text-align: center;
        }
        img {
            max-width: 100%;
            height: auto;
            margin-bottom: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .profile {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin: 20px 0;
        }
        .profile-item {
            margin: 10px;
            padding: 10px;
            background-color: #f2f2f2;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .profile-item h3 {
            margin: 0;
            font-size: 24px;
            font-weight: normal;
            margin-bottom: 10px;
        }
        .profile-item p {
            margin: 0;
            font-size: 18px;
            line-height: 1.5;
        }
        @keyframes rotate {
            from {
                transform: rotate(0);
            }
            to {
                transform: rotate(360deg);
            }
        }
        .loading {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: #fff;
            z-index: 999;
        }
        .loading-circle {
            width: 50px;
            height: 50px;
            border: 5px solid transparent;
            border-top: 5px solid black;
            border-radius: 50%;
            animation: rotate 1s linear infinite;
            margin-bottom: 20px;
        }
        .loading-text {
            display: none;
        }
    </style>
    <script>
        window.addEventListener('load', function() {
            document.body.classList.add('no-background');
            setTimeout(function() {
                document.querySelector('.loading').style.display = 'none';
                document.querySelector('.container').style.visibility = 'visible';
                document.body.classList.remove('no-background');
            }, 2000);
        });
    </script>
</head>
<body>
    <div class="loading">
        <div class="loading-circle"></div>
    </div>
    <div class="container">
        <h1>Rem - Anime Character</h1>
        <img src="https://th.bing.com/th/id/OIP.TprRZcD8sYRHwyr1alVvYgHaKn?pid=ImgDet&rs=1" alt="Rem">
        <p>Rem is a fictional character from the anime series "Re:Zero − Starting Life in Another World". She is a maid in the Roswaal mansion and serves as one of the main supporting characters in the series. Rem is known for her kind and caring personality, as well as her exceptional combat abilities.</p>
        <div class="profile">
            <div class="profile-item">
                <h3>Name</h3>
                <p>Rem</p>
            </div>
            <div class="profile-item">
                <h3>Age</h3>
                <p>18</p>
            </div>
            <div class="profile-item">
                <h3>Gender</h3>
                <p>Female</p>
            </div>
            <div class="profile-item">
                <h3>Occupation</h3>
                <p>Maid</p>
            </div>
            <div class="profile-item">
                <h3>Abilities</h3>
                <p>Exceptional combat abilities</p>
            </div>
        </div>
    </div>
</body>
</html>
