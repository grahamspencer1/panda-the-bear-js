> 1. Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead.

var profileImage = document.querySelector('.profile-image');
profileImage.src = "https://placebear.com/400/400.jpg";

//////////////////////////////////////////////////////////

> 2. Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.

var skyImage = document.querySelector('.photography');
skyImage.src = "https://placebear.com/325/225.jpg";

//////////////////////////////////////////////////////////

> 3. Select the heading that says "Panda the Bear" and change it to your own name.

var myHeading = document.querySelector('h1.highlight');
myHeading.innerText = "Graham Spencer";

//////////////////////////////////////////////////////////

> 4. Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)

var myTitle = document.querySelector('#employment h3');
myTitle.innerText = "Places That Have Fired Me";

//////////////////////////////////////////////////////////

> 5. Change the colour of the body.

var body = document.querySelector('body');
body.style.color = 'pink';
body.style.fontFamily = 'Comic Sans MS'; <!-- added to make uglier -->

//////////////////////////////////////////////////////////

> 6. Change the colour of each element using the highlight class. Use a for loop to do this.

var changeColor = document.querySelectorAll('.highlight');
changeColor.forEach(function(highlight){
  highlight.style.backgroundColor = 'maroon';
})

//////////////////////////////////////////////////////////

> 7. Change the font family of the h1 to 'monospace'.

var myHeading = document.querySelector('h1');
myHeading.style.fontFamily = "monospace";

//////////////////////////////////////////////////////////

> 8. Find a way to select the round icons in the sidebar and then change their colour.

var iconColor = document.querySelectorAll('.action-icon-bg');
iconColor.forEach(function(changeColor){
  changeColor.style.backgroundColor = 'pink';
});

//////////////////////////////////////////////////////////

> 9. Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

//////////////////////////////////////////////////////////

> 10. Change the placeholder attribute of the message field to "state your business".

//////////////////////////////////////////////////////////

> 11. Give the name field a "value" attribute of "your nemesis".

//////////////////////////////////////////////////////////

> 12. Change the value attribute of the email field to "koalathebear@gmail.com".

//////////////////////////////////////////////////////////

> 13. Change the value of the submit button on the contact form to "En garde!".

//////////////////////////////////////////////////////////

> 14. We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).

//////////////////////////////////////////////////////////

> 15. We should help Panda protect their privacy by erasing their personal details from the sidebar.
