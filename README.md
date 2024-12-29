
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login</title>
    <script defer src="login.js"></script>
</head>
<style>
    /* General Styles */
body {
    font-family: Arial, sans-serif;
    background-color: #f0f4f8;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

form {
    background: #ffffff;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    width: 100%;
    max-width: 400px;
}

h1 {
    text-align: center;
    margin-bottom: 1.5rem;
    font-size: 24px;
    color: #333;
}

label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: bold;
    color: #555;
}

input {
    width: 100%;
    padding: 0.75rem;
    margin-bottom: 1rem;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 16px;
}

button {
    width: 100%;
    background-color: #4caf50;
    color: white;
    padding: 0.75rem;
    border: none;
    border-radius: 4px;
    font-size: 16px;
    cursor: pointer;
}

button:hover {
    background-color: #45a049;
}

p {
    text-align: center;
    margin-top: 1rem;
    color: #666;
}

a {
    color: #007bff;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}

/* Responsive Design */
@media (max-width: 600px) {
    form {
        padding: 1rem;
    }

    h1 {
        font-size: 20px;
    }

    input, button {
        font-size: 14px;
    }
}
</style>
<body>
    <h1>Login</h1>
    <form id="loginForm">
        <label for="username">Username:</label>
        <input type="text" id="username" required>
        <br>
        <label for="password">Password:</label>
        <input type="password" id="password" required>
        <br>
        <button type="submit">Login</button>
    </form>
    <p>Don't have an account? <a href="signup.html">Sign up here</a></p>
    
<script>
    document.getElementById('loginForm').addEventListener('submit', function (e) {
    e.preventDefault();

    const username = document.getElementById('username').value;
    const password = document.getElementById('password').value;

    // Retrieve users from local storage
    let users = JSON.parse(localStorage.getItem('users')) || [];
    const user = users.find(user => user.username === username && user.password === password);

    if (user) {
        alert('Login successful!');
        // Set logged-in user in local storage
        localStorage.setItem('loggedInUser', JSON.stringify(user));
        // Redirect to the main application
        window.location.href = 'popo.html';
    } else {
        alert('Invalid username or password.');
    }
});
</script>
</body>
</html>
