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
