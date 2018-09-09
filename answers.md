/////// PART ONE ///////

> 1. Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead.

var profileImage = document.querySelector('.profile-image');
profileImage.src = "https://placebear.com/400/400.jpg";


> 2. Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.

var skyImage = document.querySelector('.photography');
skyImage.src = "https://placebear.com/325/225.jpg";


> 3. Select the heading that says "Panda the Bear" and change it to your own name.

var myHeading = document.querySelector('h1.highlight');
myHeading.innerText = "Graham Spencer";


> 4. Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)

var myTitle = document.querySelector('#employment h3');
myTitle.innerText = "Places That Have Fired Me";


> 5. Change the colour of the body.

var body = document.querySelector('body');
body.style.color = 'pink';
body.style.fontFamily = 'Comic Sans MS'; <!-- added to make uglier -->


> 6. Change the colour of each element using the highlight class. Use a for loop to do this.

var changeColor = document.querySelectorAll('.highlight');
changeColor.forEach(function(highlight){
  highlight.style.backgroundColor = 'maroon';
})


> 7. Change the font family of the h1 to 'monospace'.

var myHeading = document.querySelector('h1');
myHeading.style.fontFamily = "monospace";


> 8. Find a way to select the round icons in the sidebar and then change their colour.

var iconColor = document.querySelectorAll('.action-icon-bg');
iconColor.forEach(function(changeColor){
  changeColor.style.backgroundColor = 'pink';
});


> 9. Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

var idYourself = document.querySelector('#name');
idYourself.placeholder = "Identify Yourself";


> 10. Change the placeholder attribute of the message field to "state your business".

var yourBusiness = document.querySelector('#message');
yourBusiness.placeholder = "State Your Business";


> 11. Give the name field a "value" attribute of "your nemesis".

var yourNemesis = document.querySelector('#name');
yourNemesis.value = "Your Nemesis";


> 12. Change the value attribute of the email field to "koalathebear@gmail.com".

var changeEmail = document.querySelector('#email');
changeEmail.value = "koalathebear@gmail.com";


> 13. Change the value of the submit button on the contact form to "En garde!".

var enGarde = document.querySelector('#submit');
enGarde.value = "En garde!";


> 14. We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).

var disableSubmit = document.querySelector('#submit').disabled = true;


> 15. We should help Panda protect their privacy by erasing their personal details from the sidebar.

var hideDetails = document.querySelector('.bio-info');
hideDetails.parentNode.removeChild(hideDetails);


/////// PART TWO ///////

> 1. Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice. Use your googling and docs-skimming skillz to find a javaScript function that will allow you to remove elements from the DOM. (hint: there are multiple ways of doing this, but parentNode might be useful when it comes to selecting the right element)

var removeTimeTravel = document.querySelector('#time-travel');
removeTimeTravel.parentNode.removeChild(removeTimeTravel);

> 2. That drawing of Pikachu is really cute. Let’s duplicate it using cloneNode() and insert it at the bottom of the .portfolio-container using insertAdjacentHTML() or appendChild().

var pikachu = document.querySelector("#right-image img");
var clonePikachu = pikachu.cloneNode(true);
document.querySelector(".portfolio-container").appendChild(clonePikachu);

> 3. Wow, that was so satisfying I think we should do it 10 more times. Use a for loop to help you do this.



> 4. Let’s add a message about when the page was last updated. We'll do this by appending a new <li> element to the <ul> in the sidebar (you might need to refresh the page to bring back the list items that we emptied out earlier).
