#Annie-feedback-system


#INDEX.HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Annie - Customer Feedback Portal</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header class="header">
        <div class="logo">Annie</div>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#feedback">Feedback</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero-section">
        <h1>Welcome to Annie</h1>
        <p>Your trusted partner for collecting valuable customer feedback.</p>
        <a href="#feedback" class="cta-button">Give Feedback</a>
    </section>

    <section id="feedback" class="feedback-section">
        <div class="feedback-form">
            <h2>Customer Feedback</h2>
            <form id="form">
                <label for="name">Name</label>
                <input type="text" id="name" name="name" placeholder="Your Name" required>

                <label for="email">Email</label>
                <input type="email" id="email" name="email" placeholder="Your Email" required>

                <label for="rating">Rating</label>
                <select id="rating" name="rating" required>
                    <option value="">Select rating</option>
                    <option value="5">5 - Excellent</option>
                    <option value="4">4 - Good</option>
                    <option value="3">3 - Average</option>
                    <option value="2">2 - Poor</option>
                    <option value="1">1 - Very Poor</option>
                </select>

                <label for="comments">Comments</label>
                <textarea id="comments" name="comments" rows="4" placeholder="Your comments..." required></textarea>

                <button type="submit">Submit Feedback</button>
                <p class="success-message" id="success">Thank you for your feedback!</p>
            </form>
        </div>
    </section>

    <footer id="contact" class="footer">
        <p>&copy; 2025 Annie Feedback Portal. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>

</html>
 
  #STYLES.CSS
   /* General Styles */
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    padding: 0;
    background: linear-gradient(135deg, #6a11cb, #2575fc);
}

/* Header */
.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 50px;
    background: #ffffff20;
    backdrop-filter: blur(10px);
}

.logo {
    font-size: 24px;
    font-weight: bold;
    color: #fff;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: 500;
}

/* Hero Section */
.hero-section {
    text-align: center;
    color: #fff;
    padding: 80px 20px 40px;
}

.hero-section h1 {
    font-size: 3rem;
}

.hero-section p {
    font-size: 1.2rem;
    margin: 15px 0;
}

.cta-button {
    background: #fff;
    color: #2575fc;
    padding: 12px 30px;
    border-radius: 25px;
    text-decoration: none;
    font-weight: bold;
    transition: all 0.3s ease;
}

.cta-button:hover {
    background: #2575fc;
    color: #fff;
}

/* Feedback Form */
.feedback-section {
    display: flex;
    justify-content: center;
    padding: 50px 20px;
}

.feedback-form {
    background: #fff;
    padding: 30px;
    border-radius: 15px;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
    width: 100%;
    max-width: 400px;
}

.feedback-form h2 {
    text-align: center;
    color: #333;
    margin-bottom: 20px;
}

.feedback-form label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
    color: #444;
}

.feedback-form input,
.feedback-form textarea,
.feedback-form select {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
    border: 1px solid #ccc;
    border-radius: 8px;
}

.feedback-form button {
    background: #2575fc;
    color: #fff;
    padding: 12px;
    width: 100%;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    font-weight: bold;
    transition: background 0.3s ease;
}

.feedback-form button:hover {
    background: #6a11cb;
}

.success-message {
    display: none;
    text-align: center;
    color: green;
    font-weight: bold;
    margin-top: 10px;
}

/* Footer */
.footer {
    text-align: center;
    color: #fff;
    padding: 20px;
    margin-top: 50px;
    background: #ffffff20;
    backdrop-filter: blur(10px);
}



#SCRIPT.JS
document.getElementById('form').addEventListener('submit', function (e) {
    e.preventDefault();
    document.getElementById('success').style.display = 'block';
    this.reset();
});


#RESULT

<img width="478" alt="image" src="https://github.com/user-attachments/assets/84ea6c1d-b532-4153-92b0-53b571b9f979" />

 
