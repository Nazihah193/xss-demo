# xss-demo
<!DOCTYPE html>
<html>
<head>
  <title>Unsafe XSS Demo</title>
</head>
<body>
  <h2>Enter your comment:</h2>
  <form>
    <input type="text" id="userInput" placeholder="Write something..." />
    <button type="button" onclick="showComment()">Submit</button>
  </form>

  <h3>Output:</h3>
  <div id="output"></div>

  <script>
    function showComment() {
      let input = document.getElementById("userInput").value;
      document.getElementById("output").innerHTML = input;
    }
  </script>
</body>
</html>
