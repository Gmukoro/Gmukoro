# Hello, I'm Godspower (Guspiloo) 👋

<div id="typing-container">
  <p id="line1"></p>
  <p id="line2"></p>
</div>

<script>
  // Define your lines
  const lines = [
    "I am Godspower (Guspiloo).",
    "A Frontend Engineer based in Abuja, Nigeria."
  ];

  // Set up typing animation
  const typingContainer = document.getElementById("typing-container");
  let lineIndex = 0;
  let charIndex = 0;

  function type() {
    if (lineIndex < lines.length) {
      const currentLine = lines[lineIndex];
      document.getElementById(`line${lineIndex + 1}`).textContent =
        currentLine.substring(0, charIndex);
      charIndex++;

      if (charIndex > currentLine.length) {
        charIndex = 0;
        lineIndex++;
      }
    }
  }

  setInterval(type, 100); // Adjust the typing speed (milliseconds)
</script>

