Steps to send whatsapp messages on loop: -
Open Whatsapp web.
Click on the person you want to send messages on loop.
then open the browser console.
copy the code from below.
paste the code in browser console.
Hit enter then it will ask you to type your message and the number of times you want to send the message.
Done. 👍
/////////////////
var message = prompt("Enter your message", "‎");
var counter = parseInt(prompt("How many Times ?", 10));
window.InputEvent = window.Event || window.InputEvent;
var event = new InputEvent("input", { bubbles: true });
var textbox = document.getElementsByClassName("_1awRl copyable-text selectable-text")[1];
for (let index = 0; index < counter; index++) {
  textbox.innerHTML = message;
  textbox.dispatchEvent(event);
  document.getElementsByClassName("_2Ujuu")[0].click();
}
////////////////