HTML:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Webpage Title</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section class="hero">
            <h1>Welcome to Our Website</h1>
            <p>Explore our products and services</p>
            <button class="button">Get Started</button>
        </section>
        <section class="features">
            <div class="feature">
                <h2>Feature 1</h2>
                <p>Details about Feature 1</p>
            </div>
            <div class="feature">
                <h2>Feature 2</h2>
                <p>Details about Feature 2</p>
            </div>
            <div class="feature">
                <h2>Feature 3</h2>
                <p>Details about Feature 3</p>
            </div>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Your Company</p>
    </footer>
    <script src="js/script.js" defer></script>
</body>
</html>

CSS:
/* Global Styles */
:root {
    --primary-color: #123456;
    --font-family: 'Arial', sans-serif;
}

body {
    font-family: var(--font-family);
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header {
    background-color: var(--primary-color);
    padding: 20px;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

.hero {
    text-align: center;
    padding: 50px;
    background-color: #f0f0f0;
}

.hero h1 {
    font-size: 3em;
    color: var(--primary-color);
}

.hero p {
    font-size: 1.2em;
    color: #333;
}

.button {
    background: var(--primary-color);
    color: #fff;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

.features {
    display: flex;
    justify-content: space-around;
    padding: 50px;
    background-color: #fff;
}

.feature {
    text-align: center;
    width: 30%;
}

.feature h2 {
    color: var(--primary-color);
}

footer {
    text-align: center;
    background-color: #333;
    color: #fff;
    padding: 10px;
}

/* Responsive Design */
@media (max-width: 768px) {
    .features {
        flex-direction: column;
        align-items: center;
    }
    
    .feature {
        width: 80%;
        margin-bottom: 20px;
    }
}

JavaScript:
document.querySelector('.button').addEventListener('click', function() {
    alert('Button clicked!');
});
