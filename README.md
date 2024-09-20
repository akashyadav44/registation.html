  
<!DOCTYPE html>
<html>
<head>
    <title>Register Form</title>
    <link rel="stylesheet" href="css.css">
</head>
<body>
    <div class="heading">
        <h5>PMSSS</h5>
    </div>
    <div class="container hidden" id="registerContainer">
        <h2>REGISTATION</h2>
        <form id="registerForm">
            <input type="text" placeholder="Username" name="username" required>
            <input type="password" placeholder="Password" name="password" required>
            <input type="password" placeholder="Confirm Password" name="confirm_password" required>
            <button type="submit">Register</button>
            <p id="loginLink">Already have an account? <a href="login.html">Login</a></p>
        </form>
    </div>

    <script>
        // JavaScript code here
        document.getElementById("registerLink").addEventListener("click", function(e) {
            e.preventDefault();
            document.getElementById("loginForm").classList.add("hidden");
            document.getElementById("registerContainer").classList.remove("hidden");
        });

        document.getElementById("loginLink").addEventListener("click", function(e) {
            e.preventDefault();
            document.getElementById("registerContainer").classList.add("hidden");
            document.getElementById("loginForm").classList.remove("hidden");
        });
    </script>
</body>
</html>
