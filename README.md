# Ex.08 Design of Interactive Image Gallery
# Date:10.05.2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div id="image">Hover over an image below to display here.</div>
    
    <div class="gallery">
        <img class = "preview" alt = "Night Sky" src = "https://images.pexels.com/photos/1624496/pexels-photo-1624496.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover = "upDate(this)" onmouseout = "unDo()">
	<img class = "preview" alt = "Rose" src = "https://images.pexels.com/photos/736230/pexels-photo-736230.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover = "upDate(this)" onmouseout = "unDo()">
	<img class = "preview" src = "https://images.pexels.com/photos/2130610/pexels-photo-2130610.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt = "Paris" onmouseover = "upDate(this)" onmouseout = "unDo()">
        <img class = "preview" alt = "Turtle" src = "https://images.pexels.com/photos/5277693/pexels-photo-5277693.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover = "upDate(this)" onmouseout = "unDo()">
	<img class = "preview" alt = "Cute Puppy" src = "https://images.pexels.com/photos/3687770/pexels-photo-3687770.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover = "upDate(this)" onmouseout = "unDo()">
	<img class = "preview" src = "https://images.pexels.com/photos/1648377/pexels-photo-1648377.jpeg?auto=compress&cs=tinysrgb&w=600" alt = "Baby" onmouseover = "upDate(this)" onmouseout = "unDo()">
    </div>
    <script src="script.js"></script>
</body>
</html>
```
style.css
```
body{
    margin: 2%;
    border: 1px solid black;
    background-color: #b3b3b3;
}
#image{
line-height:100px;
    width: 355px;
height: 170px;
    border:5px solid black;
    margin:0 auto;
background-color: #8e68ff;
background-image: url('');
background-repeat: no-repeat;
color:#FFFFFF;
text-align: center;
background-size: 100%;
margin-bottom:25px;
font-size: 120%;
}
.preview{
    width:10%;
    margin-left:17%;
border: 9px solid black;
}
img{
    width:95%;
}
```
script.js
```
// Reference to the image container
const imageDiv = document.getElementById('image');
const originalImageUrl = ''; // Set this to the URL of your original image
const originalText = "Hover over an image below to display here."; // Original text

function upDate(previewPic) {
    // Change the background image to the source of the hovered image
    imageDiv.style.backgroundImage = `url('${previewPic.src}')`;
    
    // Update the text to the alt text of the hovered image
    imageDiv.innerHTML = previewPic.alt;
}

function unDo() {
    // Reset the background image to the original URL
    imageDiv.style.backgroundImage = `url('${originalImageUrl}')`; // Use the original image URL here
    
    // Change the text back to the original text
    imageDiv.innerHTML = originalText;
}
```
# OUTPUT:
![Screenshot 2024-12-13 190137](https://github.com/user-attachments/assets/bc710ca7-4f26-4c7b-897a-e6aa0d5e9707)
![Screenshot 2024-12-19 143727](https://github.com/user-attachments/assets/eae374ce-5a40-4866-8c5b-795227b260e8)
![Screenshot 2024-12-19 143753](https://github.com/user-attachments/assets/1b6d425b-8fde-4bdc-a7e9-6aac669dafd1)



# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
