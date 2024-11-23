# gemsvault
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GEMS - Discover Hidden Treasures</title>
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
            margin: 0 1rem;
        }

        nav ul li a {
            text-decoration: none;
            color: #5E2750;
            font-weight: bold;
            font-size: 1rem;
            text-transform: uppercase;
        }

        nav ul li a:hover {
            color: #D4AF37; /* Gold hover effect */
        }

        section {
            padding: 4rem 2rem;
            text-align: center;
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
        }

        .category a {
            text-decoration: none;
            color: #5E2750;
            font-weight: bold;
        }

        footer {
            background-color: #5E2750;
            color: #F9F6F1;
            text-align: center;
            padding: 1.5rem 0;
            margin-top: 2rem;
        }

        footer a {
            color: #D4AF37;
            text-decoration: none;
        }

        footer a:hover {
            text-decoration: underline;
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
            background-color: #D4AF37;
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
            <h1>GEMS</h1>
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
                <h3>My Friends</h3>
                <p>Connect and share recommendations.</p>
                <a href="#friends">Explore Now</a>
            </div>
        </div>
    </section>

    <!-- User Login & Friends Section -->
    <section>
        <div class="container" id="auth">
            <h2>Sign Up / Login</h2>
            <input type="email" id="email" placeholder="Email">
            <input type="password" id="password" placeholder="Password">
            <button onclick="signUp()">Sign Up</button>
            <button onclick="logIn()">Log In</button>
            <p id="error-message" style="color: red;"></p>
        </div>

        <div class="container hidden" id="dashboard">
            <h2>Welcome, <span id="username">User</span></h2>
            <p>Your Friends:</p>
            <div id="friends-list"></div>
            <input type="text" id="add-friend" placeholder="Enter username to add">
            <button onclick="addFriend()">Add Friend</button>
            <button onclick="logOut()">Log Out</button>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 GEMS | <a href="#about">About</a></p>
    </footer>

    <script type="module">
        // Include the Firebase script (same as provided earlier).
        // Firebase configuration, sign-up, login, and friends system as before.
    </script>
</body>
</html>
