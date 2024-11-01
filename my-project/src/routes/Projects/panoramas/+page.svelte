<div class="container mx-auto p-4 flex flex-col items-center">
    <!-- Text Paragraph -->
    <p class="text-lg mb-4">
      The Microscopic Scanning pipeline was the culminative project in the course Experimental Capture. In this piece, I was attempting to create a super-high fidelity scan of an object by taking a series of 1080p images and stitching them together with panorama software. I landed on
      <a href="http://www.gigapan.com/" target="_blank" style="color: blue; text-decoration: underline;">
        Gigapan Stitch
      </a>
      for it's desktop client, publishing, and hosting of large images.
    </p>
    <p style = "color:red">Note: The gigapan embeddings are a little touchy, reload the page if nothing shows below</p>
    <!-- Centered Iframe -->
    <div class="iframe-grid mb-4">
      <iframe 
        width="700" 
        height="700" 
        src="https://www.gigapan.com/embeds/1hpwpg9xugA/" 
        loading = "lazy"
        frameborder="0" 
        allowfullscreen 
        webkitallowfullscreen 
        mozallowfullscreen>
      </iframe>

    <iframe width="700" height="700" src="https://www.gigapan.com/embeds/NRpvURVyyTk/" loading = "lazy" frameborder="0" allowfullscreen webkitallowfullscreen mozallowfullscreen ></iframe>
    </div>
    <div class = "iframe-grid">
        <iframe width="700" height="700" src="https://www.gigapan.com/embeds/jevvLVvsRdU/" loading = "lazy" frameborder="0" allowfullscreen webkitallowfullscreen mozallowfullscreen ></iframe>
        <iframe width="700" height="700" src="https://www.gigapan.com/embeds/n8kwUdHzr04/" loading = "lazy" frameborder="0" allowfullscreen webkitallowfullscreen mozallowfullscreen ></iframe>
    </div>
  </div>
  

<div class="container mx-auto p-4 flex flex-col items-center">
  <p>
    My pipeline used an Axi-Draw pen plotter with realtime control from Processing in order to take microscopic photographs at regular intervals across a sample up to 4 inches. The code controlling the axi-draw was made with the help of <a href = "https://flong.com/" style="color: blue; text-decoration: underline;">Golan Levin</a> and <a href = "https://abfominaya.com/" style="color: blue; text-decoration: underline;">Angelica Bonilla-Fominalla</a>. After Scanning, the images would be stitched with the Gigapan Stitch Desktop client, where their ordering has to be input row-by-by row. The largest task of this was to reorder the capture of these images to match the expectations of Gigapan. 
  </p>
  <div class = "iframe-grid">
  <img src = "/panorama/excap_setup_diagram.png" alt = "setupdiagam" class ="iframe-grid"/>
  <img src = "/panorama/AK2A4807.JPG" alt ="showdiagram " class ="iframe-grid"/>
  </div>
  <iframe width="70%" height="600" 
  src="https://www.youtube.com/embed/5qOM6FM4ACw?si=Xv5avU5KPFw9ZnLK" 
  title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>
  </iframe>
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

  padding-top: 20px;
  padding-bottom: 20px;

}
</style>