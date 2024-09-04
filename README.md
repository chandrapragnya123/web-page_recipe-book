# web-page_recipe-book
It is a web page , which shows the different recipes 
<!DOCTYPE html>
<html>
<head>
<title>Welcome Page</title>
<style>
  /* CSS for styling */
  h1 {
    font-size: 36px; /* Increase font size */
    color: #FF5733; /* Change color */
    display: none; /* Hide initially */
  }  
  input[type="submit"] {
    background-color: #33FF66; /* Neon pink */
    color: #FF0066; /* White text */
    border: none;
    padding: 15px 25px; /* Increase button size */
    text-align: center;
    display: none; /* Hide initially */
    font-size: 30px; /* Button text size */
    border-radius: 8px; /* Rounded corners */
    cursor: pointer;
    transition: transform 0.3s ease; /* Smooth transition */
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Add shadow */
    text-transform: uppercase; /* Uppercase text */
    font-family: cursive; /* Font family */
    font-weight: bold; /* Bold font */
    text-shadow: 0 0 10px #0099CC; /* Glow effect */
  }

  input[type="submit"]:hover {
    background-color: #00ffff; /* Neon blue on hover */
    transform: translateY(-5px); /* Move button up on hover */
  }
  video {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -1;
  }
</style>
</head>
<body>
<h1><p align="center"><b style="color:red ; font-size: 40px;">Cooking: A delightful journey from ingredients to smiles</b></p></h1>
<center>
<video id="bg-video" width="1500" height="450" controls autoplay>
<source src="/html5/foo.ogg" type="video/ogg"/>
<source src="C:\Users\admin\Downloads\Flavorful Moments.mp4" type="video/mp4"/>
Your browser does not support the <video> element.
</video>
</center>

<script>
document.getElementById('bg-video').addEventListener('ended', function() {
  // Video ended, show the text and login button
  document.querySelector('h1').style.display = 'block';
  document.querySelector('input[type="submit"]').style.display = 'inline-block';
});

function redirectToLoginPage() {
  // Redirect to the login page
window.location.href = "file:///C:/Users/admin/Desktop/Web%20Dev/2le.html";
;
}
</script>

<h1><b><p align="center">Discover enchanting recipes with just a click!</p></b></h1>
<p align="center"><input type="submit" value="Login" onclick="redirectToLoginPage()"></p>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
<title>Cooking Magic</title>
<style>
  body, html {
    height: 100%;
    margin: 0;
    font-family: Arial, sans-serif;
  }
  .container {
    position: relative;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-end; /* Align items to the right */
    color: maroon;
    text-align: right; /* Align text to the right */
    padding: 20px;
    box-sizing: border-box;
  }
  video {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -1;
  }
  h1 {
    font-weight: bold;
    font-size: 40px;
    margin-bottom: 5px;
  }
  h2 {
    font-weight: bold;
    font-size: 30px;
    margin-bottom: 40px;
  }
  .continue-button {
    background-color: maroon;
    color: white;
    border: none;
    padding: 10px 20px;
    font-size: 20px;
    cursor: pointer;
    border-radius: 5px;
    transition: background-color 0.3s;
  }
  .continue-button:hover {
    background-color: #800000;
  }
</style>
</head>
<body>

<video autoplay loop muted>
  <source src="C:\Users\admin\Downloads\ezgif-5-3eeab65b83.mp4" type="video/mp4">
  Your browser does not support the video tag
</video>

<div class="container">
  <h1>Thank you for joining</h1>
  <h1> "Cooking Magic"!</h1>
  
  <button class="continue-button" id="continue-btn">Click to continue</button>
</div>

<script>
document.getElementById("continue-btn").addEventListener("click", function() {
    window.location.href = "C:/Users/admin/Desktop/Web Dev/4le.html";
});
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Josefin+Sans:ital,wght@0,400;1,200;1,300;1,600&display=swap"
        rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"
        integrity="sha512-iecdLmaskl7CVKqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBW=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />
    <title>Flavoursome Recipes</title>
</head>

<body>
    <header>
        <div class="logo">Flavoursome Recipes</div>
        <div class="nav-bar">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Recipes</a></li>
                <li><a href="#">Categories</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </div>
    </header>
    <div class="hero">
        <div class="content">
            <h4>Unleash Your Culinary Passion</h4>
            <h1>Discover Taste Sensations</h1>
            <h3>Elevate Your Cooking Game</h3>
            <div class="button">Start Cooking</div>
        </div>
    </div>
    <div class="recipe">
        <h2>Featured Recipes</h2>
        <div class="box">
            <div class="card">
                <img src="Images/Img3.jpeg" alt="">
                <div class="content">
                    <h3>North Indian Thali Recipe (Easy & Quick)</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <a href="https://hebbarskitchen.com/north-indian-thali-recipe-easy-quick/" target="_blank" class="button" onclick="speak('North Indian Thali Recipe (Easy & Quick)')">View Recipe</a>
                </div>
            </div>
            <div class="card">
                <img src="Images/Img4.jpeg" alt="">
                <div class="content">
                    <h3>Mutton Biryani</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <a href="https://www.andy-cooks.com/blogs/recipes/mutton-biryani" target="_blank" class="button" onclick="speak('Mutton Biryani')">View Recipe</a>
                </div>
            </div>
            <div class="card">
                <img src="Images/Img5.jpeg" alt="">
                <div class="content">
                    <h3>Indian Chicken Curry II</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <a href="https://www.allrecipes.com/recipe/46822/indian-chicken-curry-ii/" target="_blank" class="button" onclick="speak('Indian Chicken Curry II')">View Recipe</a>
                </div>
            </div>
            <div class="card">
                <img src="Images/Img6.jpeg" alt="">
                <div class="content">
                    <h3>Paneer Butter Masala</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <a href="https://www.cookwithmanali.com/paneer-butter-masala-recipe/" target="_blank" class="button" onclick="speak('Paneer Butter Masala')">View Recipe</a>
                </div>
            </div>
            <div class="card">
                <img src="Images/Img7.jpeg" alt="">
                <div class="content">
                    <h3>Tandoori Chicken</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <a href="https://www.simplyrecipes.com/recipes/tandoori_chicken/" target="_blank" class="button" onclick="speak('Tandoori Chicken')">View Recipe</a>
                </div>
            </div>
            <div class="card">
                <img src="Images/Img8.jpeg" alt="">
                <div class="content">
                    <h3>Veg Manchurian</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <a href="https://www.vegrecipesofindia.com/veg-manchurian-veg-manchurian-gravy/" target="_blank" class="button" onclick="speak('Veg Manchurian')">View Recipe</a>
                </div>
            </div>
            <div class="card">
                <img src="Images/Img9.jpeg" alt="">
                <div class="content">
                    <h3>Dosa</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <a href="https://holycowvegan.net/dosa-recipe/" target="_blank" class="button" onclick="speak('Dosa')">View Recipe</a>    
                 </div>
             </div>
             <!-- Add the remaining two recipe cards here -->
        </div>
    </div>

    <script>
        function speak(recipeName) {
            var synth = window.speechSynthesis;
            var utterance = new SpeechSynthesisUtterance(recipeName);
            synth.speak(utterance);
        }
    </script>
     <div class=" categories">
    <h2>categories</h2>
        <div class="box">
            <div class="ca-card">
                <img src="Images/Img10.jpeg" alt=" ">
                <div class="content">
    <h3>Main Courses</h3>
    <p>Lorem ipsum dolor sit amet,consectetur adipiscing elit.</p>
    <button>Read More</button>
                </div>
            </div>
            <div class="ca-card">
                <img src="Images/Main.jpeg" alt=" ">
                <div class="content">
    <h3>Desserts</h3>
    <p>Lorem ipsum dolor sit amet,consectetur adipiscing elit.</p>
    <button>Read More</button>               
                </div>
            </div>
            <div class="ca-card">
                <img src="Images/Dessert.jpeg" alt=" ">
                <div class="content">
    <h3>Healthy Eats</h3>
    <p>Lorem ipsum dolor sit amet,consectetur adipiscing elit.</p>
    <button>Read More</button>
                </div>
            </div>
            <div class="ca-card">
                <img src="Images/Eats.jpeg" alt=" ">
                <div class="content">
    <h3>Baking</h3>
    <p>Lorem ipsum dolor sit amet,consectetur adipiscing elit.</p>
    <button>Read More</button>
                </div>
            </div>
     </div>
</footer>
</body>
</html>
