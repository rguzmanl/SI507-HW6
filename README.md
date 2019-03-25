# JavaScript assignment

## Some useful resources
* Some [JavaScript tutorials](https://www.htmldog.com/guides/javascript/)
* The complicated [resources in the You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) series, including [your reading last week](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md)
* [A resource for CSS/style/colors](https://htmlcolorcodes.com/)  
* [An excerpt from a specific workshop site](https://witny-summer-guild-2018.github.io/day_4_exercise_2.html) (for a different audience than yourselves) which addresses some common questions about jQuery
* [The simple JSFiddle example from class](https://jsfiddle.net/2of65j8q/)
* A [W3Schools resource on JavaScript output](https://www.w3schools.com/js/js_output.asp)
* Google, Piazza, your classmates, office hours, lab time!

## Included files
* This `README.md`, which you should edit with answers to the questions
* `jsPracticeLab.html`, which you'll need to edit and try out
* `jquerylib_submit_example.html`, which you'll need to edit and try out

## Your goals for this lab

### Broadly
The aim for this lab is to practice adapting to and understanding code in a new-to-you (or not) language and its own libraries/packages -- JavaScript, in this case.

The programming skills you have built up till now are useful for *Python programming*, but, more than that, they extend to fundamentals of many kinds of programming.

This experience is *not in any way* about becoming an expert JavaScript programmer. Instead, it is about using what you *do* have experience with -- and your skills in *learning new things* that relate to programming -- in order to make educated judgments about some brand new-to-you code, even if you haven't learned in detail about it yet. That's part of what being in technology -- or even technology-adjacent -- will often mean.

### Specifically

Below are a bunch of questions and indications of things to do. For each indication of something to do with code, there is also an accompanying question to answer or brief explanation to give. 

**To complete and submit this assignment, you should:**

* Fork (and clone) this repository
* Add our instructional team as a collaborator to your fork (see instructions for adding collaborators on Canvas)
* Edit this `README.md` file with answers to the questions/prompts, briefly, using Markdown formatting so that the questions appear in bulletpoints and the answers appear clearly below each respective question, *not* as bulletpoints.
* Add all names of those who worked on this (as indicated below)
* Make the changes that are indicated below to each of the `.html` files with JavaScript programs provided. (You'll probably do this concurrently with answering questions)
* Commit (as you go) and push your changes to all three files to your GitHub forked repository.
* Submit a link to your repository on Canvas. (This HW doesn't have an autograder -- it will be graded by hand/by humans this time.)

### Important notes
* You are *more than* welcome to work together on this, but **you must <u>each</u> submit a repo to be graded on it**, so if you do work together, you should do the following:
	* Make sure each one of you understands all the work -- YOU are responsible for using and knowing this information
	* Write each person's name & uniqname who worked on the assignment together on your submitted `README.md` file (you'll see a space for this below)

* In answering questions, please make sure the formatting is clear to read and that you have updated the names of everyone who worked with you, with your name first (see below).

* In answering questions, assume all of the questions include a *explain briefly* note -- you do NOT have to, and should not, write extended paragraphs. Be as concise as you can and explain in your own words. Don't worry about "whether it's enough" -- just worry about conveying your understanding so you can read it later, or even give it to someone else, and the answers will help/make sense.

* It is not acceptable to copy and paste answers from the internet and submit them as your own. If you cite things, make sure you provide a citation, including to links. If you get information from a resource and rephrase it so you're basically explaining an idea, that's just fine for an explanatory purpose in this assignment, but you *must* cite any quotes or examples that aren't yours. 

* **For grading:** we are grading on...
	* Following the instructions
	* Approximate correctness of the code edits
	* Careful & clear answers to the questions
	* Correct answers to the questions
	* Slightly more than half the 1000 points will come from answering the questions. The rest will come from your edits to the code.

### Names of people you have worked with on this assignment
* List everyone's names and uniqnames who have worked on this assignment with you, **including your own name, but make sure YOUR name is first and bold**
* Like this: 
* **Roberto Guzman (rguzmanl)**


## Questions & code instructions

### The first questions address the `jsPracticeLab.html` file.

* **This is just an example question.**

This is what an example answer should look like. If you want to include some code, which you probably don't have to do, you can, like this:

```js
Some JavaScript code
```

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**

	- Using // like in : // var regex = /^[a-zA-Z]+$/; 

* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**

	- In the head of the html file we create a tag for script '<scropt> some code here </script>'

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**

	- alert() and console.log(). The one similar to 'print' is console.log() which I'd use instead of alert() because it is better for developers' debugging. 

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...**

	- First I commented out: // alert("hello");
	- Then I added:  alert(Date()); in line 13 of the file
		- **Note: I tried different things and all worked the same. Not sure, whether there is a correct one.**

* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and replace `A name` in the web page with your own name.**

	- Withinh the function we are calling the headder h1 and replacing its text with 'A name'. To replace 'A name', I created a variable and assigned it to the selector.
	```js
		var nm = "Roberto"
		document.querySelector('h1').innerHTML = nm;
	```

* **What does the word `document` represent in this code? Explain briefly.**

	- It refers to the html file that we are writing the javascript code in. The html file represents a web page that becomes the document object.
		- https://www.tutorialspoint.com/javascript/javascript_html_dom.htm
		- https://www.w3schools.com/jsref/dom_obj_document.asp



* **What is happening in line 12 ( 
		`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? Explain, briefly (<= 2 sentences).**

	- It is calling the item with id '#items' (which is a line of text within '<p>' the id is assigned to the '<span>' element) and then it makes it equal to the length or number of list items. The second line calls all elements of type "list" and counts them. 

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**

	- White

* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. Then edit the code to make those boxes some shade of blue, of your choosing.**

	- Because there are two tags (elements) for which we assigned some styling that allows us to see their "box" within the web page. https://learn.shayhowe.com/html-css/opening-the-box-model/
	- We are using CSS styiling in the two 'p' elements. 
	```js
		p{
		/* background-color: #b3b3b3; */
		border: 3px solid #FFFFFF;
		background-color: #3753cf;
		padding: 3%;
		font-size: 1.1em;
		line-height: 1.5;
		}
	```

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**

- Not the most efficient way but this is what I did. I created a second function copyFunction2() the execut an "oncopy" event. That function is invoked in the list element of McGill University. I added a footer and a div inside in order to display 'O Canada' closer to the bottom of the page. I used some CSS styling in order to position the text, specifically I played with the top margin. I tried to use some concepts from SI-539 but I didn't go into detail.



* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**

```js
function handleClick(){
	alert("hello");
}
```
**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```
- The code uses the javascript event "onclick" and it is applied in the object button by invoking a function that determines what happens when we click on the button. The funciton executes the alert() which is a popup window with a message.


* **Knowing what you learned from the previous question, add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears. (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**

	- Code added:
	```js
	<button onclick=handleClick() id="wow-button">Wow</button>

	'within <script>':
	function anotherClick(){
		alert("March 20, 2019");

	```

### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**

* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**

	- Because we use a conditional to determine whether we are enetring valid data. The valide data is defined in the var regex which specifies only a certain type of characters as valid. When we enter invalid data the conditional executes the CSS style for "error", and when we enter valid data the conditional executes the CSS style for "good"

* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**

	- It defines a regular expression, which defines a special search pattern, and it is used to determine whether pur input is valid or not. 
	- It means, look for a string of characters that contain a through z (both lower and upper case), and that not contain spaces at the end. 

	- **Note: consulted https://www.w3schools.com/Js/js_regexp.asp and the book by Dr. Charles Severance: Python for Everybody, Exploring Data Using Python 3.**

* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**

	- In JavaScript the statement to validate is within parentheses and the action is within curly brackets {}. The same applies for the else statement that follows. Also, indentation doesn't matter but it is a good practice to use it. JavaScript doesn't have elif, it has else if instead. 

	- In Python the if statment is all in one line without any thype of brackets, it needs a : at the end of the line and indentation matters: Same applies for the elif or else statments that follow.

* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**

	- Is the time that a line of text remains visible. 1,000 = 1 sec.

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**

```js
$(document).ready(function(){
    $("form").submit(function(event){
```
- Detects whether the document object model (DOM) is ready for JavaScript code. When it is ready, then it safely runs the function. https://learn.jquery.com/using-jquery-core/document-ready/

- It is an event (submit) that occurs when the form is submitted (click the button submit). It can only be used in form elements. https://api.jquery.com/submit/ and https://www.w3schools.com/jquery/event_submit.asp



* **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.**
	* *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now.