<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RJA-Rift Jumpers Adventures</title>
    <link rel="stylesheet" href="style.css"> <!-- Link to the external CSS file -->
</head>
<body>
    <header>
        <h1>RJA Rift Jumpers Adventures</h1>
    </header>
    <nav>
        <ul>
            <li><a href="index.html" class="nav-link"><i class="fas fa-home"></i> Home</a></li>
            <li><a href="games.html" class="nav-link"><i class="fas fa-gamepad"></i> Games</a></li>
            <li><a href="wallet.html" class="nav-link"><i class="fas fa-wallet"></i> Wallet</a></li>
            <li><a href="community.html" class="nav-link"><i class="fas fa-users"></i> Community</a></li>
            <li><a href="support.html" class="nav-link"><i class="fas fa-life-ring"></i> Support</a></li>
        </ul>
    </nav>
    <section>
        <div class="wallet">
            <h2>Welcome to My RJA Top Up Center </h2>
            <p>Manage your digital funds, purchase games, and connect with other gamers.</p>
            <p>Explore our website to discover the latest games, promotions, and community events.</p>
        </div>
        <div class="form-container">
            <h2>Login</h2>
            <form id="loginForm">
                <input type="text" id="username" placeholder="Username" required><br>
                <input type="password" id="password" placeholder="Password" required><br>
                <input type="submit" value="Login">
            </form>
            <p id="loginMessage"></p>
            <p>Don't have an account? <a href="#">Sign up</a></p>
        </div>
    </section>
    <footer>
        <p>&copy; 2024 RJA Rift Jumper Adventures. All rights reserved.</p>
    </footer>
    <script>
        document.getElementById("loginForm").addEventListener("submit", function(event) {
            event.preventDefault(); // Prevent form submission
            var username = document.getElementById("username").value;
            var password = document.getElementById("password").value;
            // Perform basic validation (you can enhance this with more checks)
            if (username === "admin" && password === "password") {
                document.getElementById("loginMessage").innerText = "Login successful!";
                // Redirect to main page
                window.location.href = "mainpage.html";
            } else {
                document.getElementById("loginMessage").innerText = "Invalid username or password.";
            }
        });
    </script>
</body>
</html>

