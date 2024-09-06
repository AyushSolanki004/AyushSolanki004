document.getElementById('imageUploadForm').addEventListener('submit', function(event) {
  event.preventDefault();

  const fileInput = document.getElementById('imageInput');
  const file = fileInput.files[0];

  if (!file) {
    alert('Please select an image.');
    return;
  }

  // Preview the uploaded image
  const reader = new FileReader();
  reader.onload = function(e) {
    const previewDiv = document.getElementById('imagePreview');
    previewDiv.innerHTML = `<img src="${e.target.result}" alt="Uploaded Image">`;
  };
  reader.readAsDataURL(file);

  // Here, you would send the image to the backend server
  // For now, we simulate the detection process
  simulateFaultDetection(file);
});

function simulateFaultDetection(image) {
  const resultText = document.getElementById('resultText');

  // Simulating an API call for fault detection (replace this with actual API)
  setTimeout(() => {
    const faultDetected = Math.random() < 0.5; // Randomly simulate fault detection
    if (faultDetected) {
      resultText.textContent = 'Fault Detected: Blade damage detected on the windmill.';
      resultText.style.color = 'red';
    } else {
      resultText.textContent = 'No Fault Detected: The windmill appears to be in good condition.';
      resultText.style.color = 'green';
    }
  }, 2000); // Simulated delay
}
