<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anurag Mishra's Profile</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to right, #d9a7c7, #fffcdc);
            margin: 0;
            padding: 0;
            color: #333;
        }
        h1 {
            text-align: center;
            font-size: 2.5rem;
            color: #0e75b6;
            animation: bounce 2s infinite;
        }
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-20px); }
            60% { transform: translateY(-10px); }
        }
        .connect-icons a {
            margin: 0 10px;
            text-decoration: none;
            transition: transform 0.2s, color 0.2s;
        }
        .connect-icons a:hover {
            transform: scale(1.2);
            color: #FF4500;
        }
        .profile-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        .skills img, .connect-icons img {
            transition: transform 0.3s;
        }
        .skills img:hover, .connect-icons img:hover {
            transform: rotate(360deg);
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #0e75b6;
            color: white;
        }
        /* Dark mode toggle */
        .toggle-dark {
            position: absolute;
            top: 10px;
            right: 20px;
            cursor: pointer;
            padding: 10px;
            background-color: #333;
            color: white;
            border: none;
            border-radius: 4px;
        }
    </style>
</head>
<body>

<!-- Toggle Dark Mode -->
<button class="toggle-dark" onclick="toggleDarkMode()">Toggle Dark Mode</button>

<div class="profile-container">
    <div id="toc">
        <ul align="center" style="list-style: none">
            <summary>
                <h1 id="greeting"></h1>
            </summary>
        </ul>
    </div>

    <!-- Connect with me section -->
    <h3 align="left">Connect with me:</h3>
    <div class="connect-icons">
        <a href="anuragmishra0521@gmail.com" target="_blank">
            <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" height="28">
        </a>
        <a href="https://www.linkedin.com/in/17AnuragMishra" target="_blank">
            <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" height="28">
        </a>
        <a href="https://twitter.com/17AnuragMishra" target="_blank">
            <img src="https://img.shields.io/badge/Twitter-000000?style=for-the-badge&logo=X&logoColor=white" height="28">
        </a>
        <a href="https://www.youtube.com/@problemscracked" target="_blank">
            <img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" height="28">
        </a>
        <a href="https://github.com/17AnuragMishra" target="_blank">
            <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" height="28">
        </a>
    </div>

    <!-- Skills Section -->
    <h3 align="left">Skills</h3>
    <div class="skills" align="left">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-plain.svg" height="28" alt="C++">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original-wordmark.svg" height="28" alt="Java">
        <img src="https://img.shields.io/badge/JavaScript-F7DF1C?logo=javascript&logoColor=white" height="28" alt="JavaScript">
        <img src="https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB" height="28" alt="React">
        <img src="https://img.shields.io/badge/Node.js-8CC84B?logo=node.js&logoColor=white" height="28" alt="Node.js">
        <!-- Additional skills -->
    </div>

    <!-- GitHub Stats Section -->
    <h3 align="left">GitHub Stats</h3>
    <div align="left">
        <img width="48%" src="https://github-readme-stats.vercel.app/api?username=17AnuragMishra&theme=react&hide_title=false&hide_rank=false&show_icons=false&include_all_commits=false&count_private=true&line_height=23" alt="GitHub stats Card" />
        <img width="48%" src="https://streak-stats.demolab.com/?user=17AnuragMishra&theme=react&hide_border=false&date_format=M+j%5B%2C+Y%5D&mode=daily&hide_total_contributions=false&hide_current_streak=false&hide_longest_streak=false&card_height=200" alt="GitHub streak Card" />
    </div>

    <!-- Footer -->
    <footer>
        &copy; 2024 Anurag Mishra | All Rights Reserved
    </footer>
</div>

<script>
    // Greet based on the time of day
    function setGreeting() {
        const now = new Date();
        const hours = now.getHours();
        let greetingMessage;

        if (hours < 12) {
            greetingMessage = "Good Morning! Anurag here...";
        } else if (hours < 18) {
            greetingMessage = "Good Afternoon! Anurag here...";
        } else {
            greetingMessage = "Good Evening! Anurag here...";
        }

        document.getElementById("greeting").innerText = greetingMessage;
    }

    setGreeting();

    // Toggle dark mode
    function toggleDarkMode() {
        document.body.classList.toggle("dark-mode");
    }
</script>
</body>
</html>
