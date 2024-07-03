<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
  /* Basic styling for the navigation menu */
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
  }
  .navbar {
    position: fixed;
    top: 0;
    width: 100%;
    background-color: #333;
    z-index: 1000;
    transition: background-color 0.3s ease;
  }
  .navbar ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    text-align: center;
  }
  .navbar li {
    display: inline;
    margin: 0 10px;
  }
  .navbar a {
    display: block;
    color: white;
    text-decoration: none;
    padding: 10px 20px;
    transition: color 0.3s ease;
  }
  .navbar a:hover {
    color: #00bcd4;
  }
</style>
<title>Interactive Navigation Menu</title>
</head>
<body>
<div class="navbar" id="navbar">
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#services">Services</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</div>

<!-- Some content to demonstrate scrolling -->
<div style="height: 1200px; padding-top: 50px;">
  <h2 id="home">Welcome to Our Website</h2>
  <p>Scroll down to see the effect on the navigation menu.</p>
</div>

<script>
  // JavaScript for changing the navbar style on scroll
  window.onscroll = function() {scrollFunction()};
  
  function scrollFunction() {
    var navbar = document.getElementById("navbar");
    if (document.body.scrollTop > 50 || document.documentElement.scrollTop > 50) {
      navbar.style.backgroundColor = "#555";
    } else {
      navbar.style.backgroundColor = "#333";
    }
  }
</script>

</body>
</html>
