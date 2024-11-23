<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GEMS Vault - Discover Hidden Treasures</title>
    <style>
        /* General Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Helvetica', Arial, sans-serif;
            background-color: #F9F6F1; /* Soft white */
            color: #5E2750; /* Deep prune */
            line-height: 1.6;
            overflow-x: hidden;
        }

        header {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(
                rgba(94, 39, 80, 0.7),
                rgba(94, 39, 80, 0.7)
            ), url('large-624x455.png') no-repeat center center/cover;
            text-align: center;
            color: #F9F6F1; /* White overlay text */
        }

        header h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            text-transform: uppercase;
        }

        header p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto;
        }

        nav {
            background-color: #F9F6F1;
            padding: 1rem 0;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
        }

        nav ul li {
            margin: 0 1.5rem;
        }

        nav ul li a {
            text-decoration: none;
            color: #5E2750;
            font-weight: bold;
            font-size: 1.1rem;
            text-transform: uppercase;
        }

        nav ul li a:hover {
            color: #003366; /* Dark blue hover effect */
        }

        section {
            padding: 4rem 2rem;
            text-align: center;
            background-color: #FFF;
        }

        section h2 {
            font-size: 2rem;
            margin-bottom: 1.5rem;
            color: #5E2750;
        }

        .categories {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .category {
            background-color: #FFF;
            border: 1px solid #DDD;
            border-radius: 8px;
            padding: 2rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }

        .category:hover {
            transform: translateY(-10px);
            box-shadow: 0 6px 12px rgba(0, 51, 102, 0.3); /* Dark blue shadow on hover */
        }

        .category a {
            text-decoration: none;
            color: #5E2750;
            font-weight: bold;
        }

        .category a:hover {
            color: #003366; /* Dark blue link hover */
        }

        .search-section {
            margin: 2rem auto;
            text-align: center;
        }

        .search-section input {
            padding: 0.8rem;
            width: 80%;
            max-width: 600px;
            margin-bottom: 1rem;
            border: 1px solid #DDD;
            border-radius: 5px;
        }

        .search-section button {
            padding: 0.8rem 2rem;
            background-color: #5E2750;
            color: #FFF;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1rem;
        }

        .search-section button:hover {
            background-color: #003366; /* Dark blue button hover */
        }

        footer {
            background-color: #5E2750;
            color: #F9F6F1;
            text-align: center;
            padding: 2rem 0;
            margin-top: 3rem;
        }

        footer a {
            color: #D4AF37;
            text-decoration: none;
            margin: 0 1rem;
            font-size: 1.2rem;
        }

        footer a:hover {
            color: #003366; /* Dark blue hover for footer links */
        }

        .container {
            max-width: 500px;
            margin: 0 auto;
            padding: 20px;
            border: 1px solid #DDD;
            border-radius: 10px;
            background: #FFF;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            margin-top: 20px;
        }

        input, button {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #CCC;
            border-radius: 5px;
        }

        button {
            background-color: #5E2750;
            color: #FFF;
            cursor: pointer;
        }

        button:hover {
            background-color: #003366; /* Dark blue button hover */
        }

        .hidden {
            display: none;
        }
    </style>
</head>
<body>
    <!-- Hero Section -->
    <header>
        <div>
            <h1>GEMS Vault</h1>
            <p>Discover hidden treasures in movies, books, and music. Curate, share, and explore a world beyond the spotlight.</p>
        </div>
    </header>

    <!-- Navigation -->
    <nav>
        <ul>
            <li><a href="#movies">Movies/Series</a></li>
            <li><a href="#books">Books</a></li>
            <li><a href="#music">Music</a></li>
            <li><a href="#collections">My Gems Collection</a></li>
            <li><a href="#friends">My Friends</a></li>
            <li><a href="#search">Search</a></li>
            <li><a href="#about">About</a></li>
        </ul>
    </nav>

    <!-- Categories Section -->
    <section id="categories">
        <h2>Explore Categories</h2>
        <div class="categories">
            <div class="category">
                <h3>Movies/Series</h3>
                <p>Discover hidden gems in cinema.</p>
                <a href="#movies">Explore Now</a>
            </div>
            <div class="category">
                <h3>Books</h3>
                <p>Find your next great read.</p>
                <a href="#books">Explore Now</a>
            </div>
            <div class="category">
                <h3>Music</h3>
                <p>Uncover rare tracks and tunes.</p>
                <a href="#music">Explore Now</a>
            </div>
            <div class="category">
                <h3>My Gems Collection</h3>
                <p>Curate and showcase your favorites.</p>
                <a href="#collections">Explore Now</a>
            </div>
            <div class="category">
                <h3>Search</h3>
                <p>Find treasures from YouTube, Netflix, and Spotify.</p>
                <a href="#search">Search Now</a>
            </div>
        </div>
    </section>

    <!-- Search Section -->
    <section id="search">
        <h2>Search for Gems</h2>
        <div class="search-section">
            <input type="text" id="search-query" placeholder="Search for a movie, book, or song...">
            <button onclick="search()">Search</button>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 GEMS Vault | <a href="#about">About Us</a></p>
        <p>
            <a href="https://twitter.com/gemsvault" target="_blank">Twitter</a>
            <a href="https://instagram.com/gemsvault" target="_blank">Instagram</a>
            <a href="https://facebook.com/gemsvault" target="_blank">Facebook</a>
        </p>
    </footer>

    <script>
        // Search Functionality
        function search() {
            const query = document.getElementById("search-query").value;
            if (!query) {
                alert("Please enter a search term!");
                return;
            }
            window.open(`https://www.google.com/search?q=${query}`, "_blank");
        }
    </script>
</body>
</html>
