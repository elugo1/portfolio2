<div class="container mx-auto p-4 flex flex-col items-center">
    <!-- Text Paragraph -->
    <p class="text-lg mb-4">
      The Microscopic Scanning pipeline was the culminative project in the course Experimental Capture. In this piece, I was attempting to create a super-high fidelity scan of an object by taking a series of 1080p images and stitching them together with panorama software. I landed on Gigapan Stitch
      <a href="http://www.gigapan.com/" target="_blank" style="color: blue; text-decoration: underline;">
        Gigapan Stitch
      </a>
      for its destop client, publishing, and hosting of large images.

    </p>
  
    <!-- Centered Iframe -->
    <div class="iframe-grid mb-4">
    
      <iframe 
        width="700" 
        height="700" 
        src="https://www.gigapan.com/embeds/1hpwpg9xugA/" 
        frameborder="0" 
        allowfullscreen 
        webkitallowfullscreen 
        mozallowfullscreen>
      </iframe>

    <iframe width="700" height="700" src="https://www.gigapan.com/embeds/NRpvURVyyTk/" frameborder="0" allowfullscreen webkitallowfullscreen mozallowfullscreen ></iframe>
    </div>
    <div class = "iframe-grid">
        <iframe width="700" height="700" src="https://www.gigapan.com/embeds/jevvLVvsRdU/" frameborder="0" allowfullscreen webkitallowfullscreen mozallowfullscreen ></iframe>
        <iframe width="700" height="700" src="https://www.gigapan.com/embeds/n8kwUdHzr04/" frameborder="0" allowfullscreen webkitallowfullscreen mozallowfullscreen ></iframe>
    </div>
  </div>
  
  <style>
    .video-container {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100%; /* Makes the container take up full width */
      overflow: hidden;
    }
    .container {
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .iframe-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr); /* 2 columns for a 2x2 grid */
    gap: 20px; /* Adjust spacing between iframes */
  }
  </style>
  