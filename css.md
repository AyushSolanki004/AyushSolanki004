* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f9;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  width: 400px;
  text-align: center;
}

h1 {
  font-size: 24px;
  margin-bottom: 20px;
}

form {
  margin-bottom: 20px;
}

input[type="file"] {
  padding: 10px;
  border-radius: 5px;
  border: 1px solid #ddd;
  margin-bottom: 10px;
  width: 100%;
}

button {
  padding: 10px 20px;
  border-radius: 5px;
  background-color: #007bff;
  color: white;
  border: none;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}

#imagePreview {
  margin-bottom: 20px;
}

#imagePreview img {
  max-width: 100%;
  height: auto;
  display: block;
  margin: 0 auto;
}

#resultSection {
  margin-top: 20px;
}

#resultText {
  font-weight: bold;
}
