<script>
  // No specific script needed for layout purposes
</script>

<div class="bio-layout">
  <img src="/thumbnail_images/profile_image.png" alt="Bio" class="bio-photo" />

  <p class="para-1">
  My name is Em or Emmanuel I am a creative technologist based in Pittsburgh, PA. 
  I am currently staff at the Carnegie Mellon School of Art as an intern for the Physical Computing and Digital Fabrication Labs
  <br>
  <p/> 
  <p class = "para-2">I often make work that deals with perspectives of death through the eyes of decomposers, and use computer graphics to simulate these relationships.
  I am very interested in alternative forms of capture and representing data, as well as using found footage to create simulations or interactive experiences. 
  Creative Coding platforms like Touchdesigner, Processing, and p5.js have helped me realize my ideas along the way, and I am always looking for ways to engage with software communities.
  </p>

  <div class="education-section">
    <h1 class="font-extrabold">Education</h1>
    <p class="para-1 indent-0">2020-2024 <br/>BFA, School of Art, <a href="https://art.cmu.edu/" style ="text-decoration: underline; color:#475569;">Carnegie Mellon University</a>
    <h1 class="font-extrabold">Awards & Grants</h1>
    <p class = " text-black indent-0" ><a href="https://art.cmu.edu/news/alumni-news/emmanuel-lugo-ken-meyer-award/" style ="text-decoration: underline; color:#475569;">Ken Meyer Professional Studio Development Award</a>, 2024<br> School of Art Award, 2024 <br> The Frank Ratchye Further Fund, 2023 & 2022</p>
    <h1 class = "font-extrabold">Teaching</h1> 
    <p class="text-black indent-0"> Teaching Assistant/60-212:Creative Code  Fall 2023 & 2024<br>
    Touchdesigner Teaching Assistant/ <a href="https://live.artandcode.org/" style ="text-decoration: underline; color:#475569;">LIVE Art&&Code @ the STUDIO for Creative Inquiry, Fall 2023</a>
    </p>
  </div>
</div>

<style>
  .bio-layout {
    display: grid;
    grid-template-columns: 1fr 1.5fr 1fr; /* Equal width columns */
    grid-template-rows: auto auto; /* Two rows: one for image + top paragraphs, another for paragraph 1 */
    gap: 20px;
    padding: 20px;
  }

  .bio-photo {
    grid-column: 1 / 2; /* Image in the first column */
    grid-row: 1 / 2; /* Image starts at the top */
    width: 100%;
    max-width: 500px;
    border-radius: 20px;
  }
  .education-section {
    grid-column: 2 / 3; /* Place the education content in the second column */
    grid-row: 1 / 2; /* In the first row */
  }

  .para-1 {
    grid-column: 1 / 4; /* Paragraph spans all columns */
    grid-row: 2 / 3; /* Starts below the image */
    color: black;
    width: 50%;
  }

  h1 {
    grid-column: 2 / 3; /* The header will be in the second column */
    grid-row: 1 / 2; /* The header starts in the first row */
    color:black;
    /* padding-bottom: 5px; Add a little padding to separate from the paragraph */
  }

   .para-2 {
    grid-column: 1 / 4; /* Paragraph spans all columns */
    grid-row: 3 / 3; /* Starts below the image */
    color: black;
    width: 50%;
  } 

  .para-3 {
    grid-column: 3 / 4; /* Paragraph 3 in the third column */
    grid-row: 1 / 2; /* This starts in the first row */
    color: black;
  }
</style>
