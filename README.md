# Css-flexbox-Layout-
/*index-flexbox.html*/
<!DOCTYPE html>
<html>
<html lang="en">
<head>
  <meta http-equiv="CONTENT-TYPE" content="text/html; charset=UTF-8">
   <title>This is my Flexbox Layout</title>
    <link rel="stylesheet" href="flexbox.css">
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
        <section class="content-section">
            <h2>First Section</h2>
            <p>This is for the content of the First section. I used Flexbox here.</p>
        </section> 
       <section class="content-section">
            <h2>Second Section</h2>
            <p>This is for the content of the Second section. I used Flexbox here</p>
        </section>
        <section class="content-section">
            <h2>Third Section</h2>
            <p>This is for the content of the Third section. I used Flexbox here.</p>
        </section>
    </main>
 <footer>
        <p>&copy; 2025 My Webpage Using Flexbox</p>
    </footer>
</body>
</html>


/*flexbox.css*/
body {
    font-family: sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

header {
    background-color: #333;
    color: #fff;
    padding: 1em 0;
}

nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex; 
    justify-content: space-around;
}

nav a {
    color: #fff;
    text-decoration: none;
    padding: 1em;
    display: block;
}

main {
    padding: 1em;
}

.content-section {
    background-color: #fff;
    padding: 1em;
    margin-bottom: 1em;
    border-radius: 5px;
}

footer {
    text-align: center;
    padding: 1em;
    background-color: #333;
    color: #fff;
}

main {
    display: flex;
    flex-direction: column; 
}

@media (min-width: 768px) { 
    main {
        flex-direction: row; 
        flex-wrap: wrap; 
    }

    .content-section {
        width: calc(33.33% - 2em);
        margin: 1em;
    }
}

@media (min-width: 992px) { 
    nav ul {
        justify-content: flex-start;
        padding-left: 2em;
    }
}

