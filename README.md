# <!DOCTYPE html>
<html>
<body>
  <h1>Angela, will you be my Valentine?</h1>
  <button id="yesBtn" onclick="escalateYes()">Yes</button>
  <button id="noBtn" onclick="changeQuestion()">No</button>
  <p id="question"></p>

<script>
let count = 0;
const questions = [
  "Angela, will you be my Valentine?",
  "No? Okay... Will you be my Valentine?",
  "No? Hmm... Will you be my Valentine?",
  "No? Aw... Will you be my Valentine?",
  "No? 😄 Will you be my Valentine?",
  "No? 💖 Will you be my Valentine?",
  "No? 🥺 Will you be my Valentine?",
  "😍 Can't say no now! Will you be my Valentine?"
];
const yesOptions = [
  "Yes",
  "Yes!",
  "YES!",
  "YES PLEASE!",
  "YES PLEASE SO MUCH!",
  "Y E S  F O R  S U R E!",
  "YEEEEEEEEES!",
  "Y E S  I  W I L L  B E  Y O U R  V A L E N T I N E!"
];

function changeQuestion() {
  if (count < questions.length - 1) {
    count++;
    document.getElementById("question").innerText = questions[count];
    document.getElementById("yesBtn").innerText = yesOptions[count];
  }
}

function escalateYes() {
  alert("YAY! 💖");
  // Add more actions here (like redirecting or showing a message)
}
</script>
</body>
</html>
