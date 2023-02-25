# 🌟 New Thing 01 | Upload Image Using JS

## 🛠️ Tools Utilized
I used HTML, CSS, and JS to create all the design.

## 📝 Description
The styling aspect was done by CSS, but the main thing was creating a JS function that will allow users to upload an image from their device. To create the JS function, we select the displayed image and input tag using their respective IDs. Then we create a function with `input.onchange`. Next, we create a URL object and give the URL of the selected image to the displayed image, so the selected image will be displayed on the webpage.

## 🎓 Learning
I learned how to access the files of input tag using JS. I got familiar with `URL.createObjectURL`, which allows me to display images on the webpage.

## 🔗 Link
I've uploaded the code at my CodePen. You can check it out here:
https://codepen.io/farmanali6349/pen/wvEzRro

Note: Use the code at your local setup, as the image will not be shown online.

## JS Code
```javascript
let profilePic = document.getElementById('profile-pic');
let inputFile = document.getElementById('input-file');

inputFile.onchange = function () {
    profilePic.src = URL.createObjectURL(inputFile.files[0]);
}
