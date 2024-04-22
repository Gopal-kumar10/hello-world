<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>javascript</title>
<style>
/* Internal CSS */
body {
  font-family: Arial, sans-serif;
}

.container {
  text-align: center;
  margin-top: 100px;
}

.button {
  padding: 10px 20px;
  background-color: #007bff;
  color: #fff;
  border: none;
  cursor: pointer;
  border-radius: 5px;
}

.button:hover {
  background-color: #0056b3;
}

</style>
</head>
<body>

<div class="container">
  <button class="button" onclick="showDialog()">Show Dialog Box</button>
</div>

<script>
// Internal JavaScript
function showDialog() {
  var name = prompt("Please enter your name:", "GOPAL KUMAR");
  if (name != null && name != "") {
    var confirmation = confirm("RADHE RADHE  " + name + "! Are you sure you want to proceed?");
    if (confirmation) {
      alert("Welcome, " + name + "! You have successfully proceeded.");
    } else {
      alert("Action cancelled.");
    }
  } else {
    alert("You didn't provide your name. Action cancelled.");
  }
}
</script>

</body>
</html>
