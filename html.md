!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fault Detection in Devices</title>
  <link rel="stylesheet" href="mecia.css">
</head>
<body>
  <div class="container">
    <h1>Fault Detection in Windmills</h1>
    <p>Upload an image of the windmill to detect faults:</p>

    <form id="imageUploadForm">
      <input type="file" id="imageInput" accept="image/*" required>
      <button type="submit">Detect Fault</button>
    </form>

    <div id="imagePreview">
      <p>No image uploaded yet.</p>
    </div>

    <div id="resultSection">
      <h2>Detection Result:</h2>
      <p id="resultText">No results yet.</p>
    </div>
  </div>

  <script src="script.js" charset="UTF-8" ></script>
</body>
</html>
