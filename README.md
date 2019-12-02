# forms

Capture input when a form is submitted:

<form id="some-form">
  <label for="some-input">Your input:</label>
  <input id="some-input" type="text">

  <button type="submit" class="btn">Submit!</button>
</form>
$("form#some-form").submit(function(event) {
  var someInput = $("input#some-input").val()

  event.preventDefault();
});
If you submit your form and then there's a ? at the end of the address bar, you forgot to put event.preventDefault();, or you attached your event listener to the wrong form.

Replace text:

$(".some-class").text("New text");
Variables defined with var are scoped to the function in which they are defined. Omitting var creates a global variable and is a bad practice.
