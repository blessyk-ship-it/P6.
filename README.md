
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>QuizHive - Positioning Elements</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #f4f1ff;
        }

        /* Header */
        header {
            background-color: #291653;
            color: white;
            text-align: center;
            padding: 25px;
        }

        header h1 {
            color: #ffcc4d;
            font-size: 35px;
        }

        header p {
            margin-top: 10px;
        }

        /* Navigation */
        nav {
            background-color: #493078;
            display: flex;
            justify-content: center;
            gap: 30px;
            padding: 15px;
            position: sticky;
            top: 0;
            z-index: 10;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        /* Main Content */
        .content {
            text-align: center;
            padding: 25px;
        }

        .content h2 {
            color: #493078;
            margin-bottom: 10px;
        }

        /* Positioning Container */
        .position-box {
            position: relative;
            width: 90%;
            max-width: 900px;
            height: 400px;
            margin: 30px auto;
            background: linear-gradient(135deg, #dcd0ff, #fce9ff);
            border: 3px solid #493078;
            border-radius: 15px;
        }

        /* Four Corner Elements */
        .corner {
            position: absolute;
            background-color: #493078;
            color: white;
            padding: 15px;
            border-radius: 8px;
            font-weight: bold;
        }

        .top-left {
            top: 15px;
            left: 15px;
        }

        .top-right {
            top: 15px;
            right: 15px;
        }

        .bottom-left {
            bottom: 15px;
            left: 15px;
        }

        .bottom-right {
            bottom: 15px;
            right: 15px;
        }

        /* Center Section */
        .center {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: white;
            color: #291653;
            padding: 25px;
            border-radius: 12px;
            text-align: center;
            width: 45%;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
        }

        .center h2 {
            margin-bottom: 10px;
        }

        /* Button */
        button {
            background-color: #493078;
            color: white;
            border: none;
            padding: 12px 20px;
            border-radius: 6px;
            margin-top: 15px;
            cursor: pointer;
        }

        button:hover {
            background-color: #ffcc4d;
            color: #291653;
        }

        /* Footer */
        footer {
            background-color: #291653;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 30px;
        }

        /* Responsive Design */
        @media (max-width: 600px) {

            nav {
                flex-wrap: wrap;
                gap: 15px;
            }

            .position-box {
                height: 350px;
            }

            .corner {
                font-size: 11px;
                padding: 8px;
            }

            .center {
                width: 55%;
                padding: 15px;
                font-size: 12px;
            }
        }

    </style>
</head>

<body>

    <!-- Header -->
    <header>
        <h1>QuizHive 🐝</h1>
        <p>Gamified Quizzes for Interactive Learning</p>
    </header>

    <!-- Navigation -->
    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
    </nav>

    <!-- Main Content -->
    <div class="content" id="home">

        <h2>Welcome to QuizHive!</h2>

        <p>
            Learn new things through fun and
            interactive quizzes.
        </p>

    </div>

    <!-- Positioning Layout -->
    <div class="position-box">

        <div class="corner top-left">
            Top Left
        </div>

        <div class="corner top-right">
            Top Right
        </div>

        <div class="corner bottom-left">
            Bottom Left
        </div>

        <div class="corner bottom-right">
            Bottom Right
        </div>

        <!-- Centered Element -->
        <div class="center" id="about">

            <h2>QuizHive</h2>

            <p>
                Learn, Play and Grow with
                interactive quizzes!
            </p>

            <button onclick="alert('Welcome to QuizHive!')">
                Get Started
            </button>

        </div>

    </div>

    <!-- Services -->
    <div class="content" id="services">

        <h2>Our Services</h2>

        <p>
            Fun Quizzes | Interactive Learning |
            Knowledge Improvement
        </p>

    </div>

    <!-- Footer -->
    <footer id="contact">
        <p>© 2026 QuizHive. All Rights Reserved.</p>
        <p>Learn • Play • Grow</p>
    </footer>

</body>
</html>

