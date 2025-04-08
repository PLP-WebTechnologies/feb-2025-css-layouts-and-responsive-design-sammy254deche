# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨



####html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Webpage</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <nav class="navbar">
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
  <main class="content">
    <section class="hero">Welcome to My Website!</section>
    <section class="info">Here is some information.</section>
  </main>
  <footer class="footer">
    © 2025 Samuel Deche. All rights reserved.
  </footer>
</body>
</html>
```
<link>

/* General Styles */
body {
  margin: 0;
  font-family: Arial, sans-serif;
}

/* Navigation Bar */
.navbar {
  background-color: #333;
  color: #fff;
  display: flex;
  justify-content: center;
  padding: 1rem;
}

.navbar ul {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}

.navbar ul li {
  margin: 0 1rem;
}

.navbar ul li a {
  color: white;
  text-decoration: none;
}

/* Flexbox Layout for Content */
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 2rem;
}

.hero {
  background-color: #f4f4f4;
  padding: 2rem;
  text-align: center;
}

.info {
  margin-top: 1rem;
  padding: 2rem;
  background-color: #e0e0e0;
}

/* Footer */
.footer {
  background-color: #333;
  color: #fff;
  text-align: center;
  padding: 1rem;
}

/* Media Queries */
@media (min-width: 768px) {
  .content {
    flex-direction: row;
    justify-content: space-around;
  }
}