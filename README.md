# Vasundhara shivhare
..

    while stack:
        vertex = stack.pop()  # Pop a vertex from the stack

        if vertex not in visited:
            visited.add(vertex)  # Mark it as visited
            print(vertex)  # Process the current vertex

            # Add unvisited neighbors to the stack
            for neighbor in reversed(graph[vertex]):  # Reverse to maintain order
                if neighbor not in visited:
                    stack.append(neighbor)

# Example usage
print("DFS Recursive:")
dfs_recursive(graph, 'A')

print("\nDFS Iterative:")
dfs_iterative(graph, 'A')

Output
Running the example code will produce the following output:

mathematica
Copy code
DFS Recursive:
A
B
D
E
F
C

DFS Iterative:
A
B
D
E
F
C
Both methods will 

4:- Creating a simple website with a welcoming message, a brief description, and navigation links is straightforward. Below is an example implementation using HTML and CSS.

HTML Structure
We'll create a basic structure with a homepage, an about page, a contact page, and a blog page.

index.html (Homepage)
html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to My Simple Website</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
                <li><a href="blog.html">Blog</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h2>Welcome!</h2>
            <p>This is a simple website created to demonstrate basic HTML and CSS features.</p>
            <p>Explore the pages to learn more about us!</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 My Simple Website</p>
    </footer>
</body>
</html>
about.html (About Page)
html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Us</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>About Us</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
                <li><a href="blog.html">Blog</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h2>Our Story</h2>
            <p>We are dedicated to providing the best service possible. Our journey began in 2020...</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 My Simple Website</p>
    </footer>
</body>
</html>
contact.html (Contact Page)
html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Contact Us</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
                <li><a href="blog.html">Blog</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h2>Get in Touch</h2>
            <p>You can reach us via email at contact@example.com or through our social media channels.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 My Simple Website</p>
    </footer>
</body>
</html>
blog.html (Blog Page)
html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Our Blog</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
                <li><a href="blog.html">Blog</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h2>Latest Posts</h2>
            <p>Stay tuned for our latest updates and articles!</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 My Simple Website</p>
    </footer>
</body>
</html>
CSS Styling (styles.css)
css
Copy code
* {
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #0073e6;
    color: white;
    padding: 1rem;
    text-align: center;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 1rem;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    padding: 2rem;
}

footer {
    text-align: center;
    padding: 1rem;
    background-color: #f1f1f1;
}

5:- Creating a responsive social media platform requires a combination of HTML for structure, CSS for styling, and JavaScript for interactivity. Below is a basic implementation that showcases a simple social media interface, complete with swipe gestures for mobile navigation.

HTML Structure
Here's a simple HTML layout for the platform:

html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Social Media Platform</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Social Media</h1>
        <nav>
            <ul>
                <li><a href="#" id="home">Home</a></li>
                <li><a href="#" id="profile">Profile</a></li>
                <li><a href="#" id="messages">Messages</a></li>
            </ul>
        </nav>
    </header>
    <main id="content">
        <section id="homeSection" class="active">
            <h2>Home Feed</h2>
            <p>Welcome to your feed!</p>
        </section>
        <section id="profileSection">
            <h2>Your Profile</h2>
            <p>Profile information goes here.</p>
        </section>
        <section id="messagesSection">
            <h2>Your Messages</h2>
            <p>No new messages.</p>
        </section>
    </main>
    <script src="script.js"></script>
</body>
</html>

CSS Styles
Add the following CSS to style the platform and ensure it is responsive:

css
Copy code
/* styles.css */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #0073e6;
    color: white;
    padding: 10px;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

main {
    padding: 20px;
}

section {
    display: none;
}

section.active {
    display: block;
}

/* Responsive styles */
@media (max-width: 600px) {
    nav ul li {
        display: block;
        margin: 10px 0;
    }

    main {
        padding: 10px;
    }
}

JavaScript Functionality
This JavaScript will handle the navigation and swipe gestures:

javascript
Copy code
// script.js
document.addEventListener("DOMContentLoaded", () => {
    const sections = document.querySelectorAll('main > section');
    let currentIndex = 0;

    function showSection(index) {
        sections.forEach((section, i) => {
            section.classList.toggle('active', i === index);
        });
    }

    document.querySelectorAll('nav a').forEach((link, index) => {
        link.addEventListener('click', (event) => {
            event.preventDefault();
            currentIndex = index;
            showSection(currentIndex);
        });
    });

    // Swipe Gesture Functionality
    let startX;
    
    main.addEventListener('touchstart', (event) => {
        startX = event.touches[0].clientX;
    });

    main.addEventListener('touchmove', (event) => {
        const moveX = event.touches[0].clientX;
        const difference = startX - moveX;

        if (difference > 50) { // Swipe Left
            if (currentIndex < sections.length - 1) {
                currentIndex++;
                showSection(currentIndex);
            }
        } else if (difference < -50) { // Swipe Right
            if (currentIndex > 0) {
                currentIndex--;
                showSection(currentIndex);
            }
        }
    });

    // Show the initial section
    showSection(currentIndex);
});

