<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rooptech-like Website</title>
    <style>
        /* Resetting default styles and setting up base styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }

        .container {
            width: 80%;
            margin: 0 auto;
            overflow: hidden;
        }

        header {
            background: #333;
            color: #fff;
            padding-top: 30px;
            min-height: 70px;
            border-bottom: #007bff 3px solid;
        }

        header h1 {
            float: left;
            margin: 0;
        }

        header nav {
            float: right;
            margin-top: 10px;
        }

        header nav ul {
            list-style: none;
        }

        header nav ul li {
            display: inline;
            margin-left: 20px;
        }

        header nav ul li a {
            color: #fff;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        header nav ul li a:hover {
            color: #007bff;
        }

        .hero {
            background: #007bff;
            color: #fff;
            padding: 80px 0;
            text-align: center;
        }

        .hero h2 {
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.2em;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            background: #333;
            color: #fff;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s ease;
        }

        .btn:hover {
            background: #007bff;
        }

        .services {
            padding: 50px 0;
            text-align: center;
            background-color: #fff;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
            border-radius: 8px;
            margin-bottom: 40px;
        }

        .services h2 {
            margin-bottom: 30px;
            color: #333;
        }

        .service {
            margin-bottom: 30px;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
            text-align: left;
            transition: box-shadow 0.3s ease;
        }

        .service:hover {
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        .service h3 {
            margin-bottom: 10px;
            color: #007bff;
        }

        .service img {
            max-width: 100%;
            border-radius: 5px;
            margin-bottom: 10px;
        }

        .about-us {
            padding: 50px 0;
            text-align: center;
        }

        .about-us h2 {
            margin-bottom: 30px;
            color: #333;
        }

        .about-us p {
            font-size: 1.1em;
            color: #555;
            margin-bottom: 20px;
            text-align: left;
        }

        .about-us .toggle-btn {
            background-color: #007bff;
            color: #fff;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .about-us .toggle-btn:hover {
            background-color: #0056b3;
        }

        .hidden-content {
            display: none;
            margin-top: 20px;
            text-align: left;
        }
        
        .hidden-content.active {
            display: block;
        }

        footer {
            background: #333;
            color: #fff;
            text-align: center;
            padding: 10px 0;
            position: absolute;
            width: 100%;
            bottom: 0;
        }

        /* Contact Form Styles */
        #contact {
            background-color: #f9f9f9;
            padding: 80px 0;
        }

        #contact .container {
            text-align: center;
        }

        #contact h2 {
            margin-bottom: 20px;
            color: #333;
        }

        #contact p {
            font-size: 1.1em;
            color: #555;
            margin-bottom: 40px;
        }

        #contact form {
            max-width: 600px;
            margin: 0 auto;
            padding: 30px;
            background-color: #fff;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
            border-radius: 8px;
        }

        #contact form label {
            display: block;
            margin-bottom: 10px;
            color: #333;
            font-weight: bold;
        }

        #contact form input[type="text"],
        #contact form input[type="email"],
        #contact form textarea {
            width: calc(100% - 20px);
            padding: 12px;
            margin-bottom: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1em;
            transition: border-color 0.3s ease;
        }

        #contact form textarea {
            resize: vertical;
            min-height: 120px;
        }

        #contact form input[type="text"]:focus,
        #contact form input[type="email"]:focus,
        #contact form textarea:focus {
            border-color: #007bff;
            outline: none;
        }

        #contact form button[type="submit"] {
            background-color: #007bff;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            font-size: 1em;
        }

        #contact form button[type="submit"]:hover {
            background-color: #0056b3;
        }

        @media (max-width: 768px) {
            .container {
                width: 90%;
            }

            #contact form {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Rooptech</h1>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <h2>Welcome to Rooptech</h2>
            <p>Your source for cutting-edge technology solutions.</p>
            <a href="#services" class="btn">Get Started</a>
        </div>
    </section>

    <section id="services" class="services">
        <div class="container">
            <h2>Our Services</h2>
            <div class="service">
                <img src="web img" alt="Web Development">
                <h3>Web Development</h3>
                <p>We create responsive and user-friendly websites.</p>
            </div>
            <div class="service">
                <img src="app img" alt="Mobile Apps">
                <h3>Mobile Apps</h3>
                <p>Custom mobile applications for your business needs.</p>
            </div>
            <div class="service">
                <img src="consult img" alt="Consulting">
                <h3>Consulting</h3>
                <p>Expert advice to help your business grow.</p>
            </div>
        </div>
    </section>

    <section id="about" class="about-us">
        <div class="container">
            <h2>About Us</h2>
            <p>Rooptech is dedicated to providing innovative technology solutions to our clients.</p>
            <button class="toggle-btn">Read More</button>
            <div class="hidden-content">
                <p>We strive to deliver high-quality services that meet the unique needs of each business we work with. Our team of experts is committed to excellence and customer satisfaction.</p>
                <p>Founded in [year], Rooptech has grown to become a trusted partner for businesses looking to leverage technology for growth and efficiency.</p>
            </div>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <p>Feel free to get in touch with us for any inquiries or business proposals.</p>
            <form>
                <label for="name">Name:</label><br>
                <input type="text" id="name" name="name" required><br>
                <label for="email">Email:</label><br>
                <input type="email" id="email" name="email" required><br>
                <label for="message">Message:</label><br>
                <textarea id="message" name="message" required></textarea><br>
                <button type="submit">Submit</button>
            </form>
        </div>
    </section>


    <script>
        // Smooth scrolling effect for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();

                const sectionId = this.getAttribute('href').substring(1);
                const section = document.getElementById(sectionId);

                if (section) {
                    section.scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Toggle button for 'About Us' section
        const toggleBtn = document.querySelector('.toggle-btn');
        const hiddenContent = document.querySelector('.hidden-content');

        toggleBtn.addEventListener('click', function() {
            hiddenContent.classList.toggle('active');
            if (hiddenContent.classList.contains('active')) {
                toggleBtn.textContent = 'Read Less';
            } else {
                toggleBtn.textContent = 'Read More';
            }
        });
    </script>
</body>
</html>

![image](file:///C:/Users/Akash%20R/Downloads/css%20project/css%20project.html)
![image](https://github.com/akasharuna003/cssproject/blob/main/Screenshot%202024-07-04%20105128.png)
![image](https://github.com/akasharuna003/cssproject/blob/main/Screenshot%202024-07-04%20105036.png)
