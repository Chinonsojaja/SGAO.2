# SGAO.2
<!DOCTYPE html>

<head>
<script src="/pictures/jquery.js"></script>
<style>
</style>
</head>

<body>
<div class="prompt"></div>
<button>Next</button>
<script>
// List of prompts for the user
var prompts = [
	'Type your pet name',
	'Type your favourite movie',
	'Type your profession',
   ];

var answers=[];
// Keep track of current prompt we're on
var currentPrompt = 0;

// A function that will call the next prompt
var nextPrompt = function() {
  //if there's no answer in the form
  if (currentPrompt != 0){
    answers.push($('input').val());
  }
	// if there is a next prompt
	if (currentPrompt < prompts.length) {
		// put first prompt in all html elements with class 
		$('.prompt').html(prompts[currentPrompt] +'<br><input type="text">');
		// move the next prompt into variable currentPrompt 
		currentPrompt = currentPrompt + 1;
	}
	//or else if we're at the end of the array
	else {
		// put a new message into the html.
		showFinal();
	}
}

//puts user answers into HTML
var showFinal = function() {
  $('.prompt').html(answers[0]+' '+answers[1]+' '+answers[2]);
}
// run nextPrompt function when button is clicked
$('button').click(function() {
	nextPrompt();
});

// Show the first prompt as soon as js loads
nextPrompt();
</script>

</body>
