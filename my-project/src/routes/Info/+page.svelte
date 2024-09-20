<!-- src/routes/Bio/+page.svelte -->
<script>
  // No specific script needed for layout purposes
</script>

<div class="bio-layout">
  <img src="/thumbnail_images/profile_image.png" alt="Bio" class="bio-photo" />

  <p class="para-1">Emmanuel Lugo is a Creative Technologist based in Pittsburgh, PA. He often creates interactive pieces and autonomous simulations that mimic the process of Death.
    He hopes that by mimicing and documenting the processes of death from a biological point of view can channel feelings of greif into 
  </p>
  <h1 class = "font-extrabold"> Education</h1>
  <p class="para-2">Education 
  <!-- </p> -->
  <p class="para-3">Paragraph 3: This is the third paragraph, and it will also start at the top next to the image.</p>
</div>

<style>
  .bio-layout {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr; /* Image column and two paragraph columns */
    grid-template-rows: auto 1fr; /* Two rows: one for image + top paragraphs, another for paragraph 1 */
    gap: 20px;
    padding: 20px;
  }

  .bio-photo {
    grid-column: 1 / 2; /* Image in the first column */
    grid-row: 1 / 2; /* Image starts at the top */
    width: 100%; /* Adjust image size */
    max-width: 500px; /* Ensure the image fits within the first column */
    border-radius: 20px;
  }

  .para-1 {
    grid-column: 1 / 2; /* Paragraph 1 spans the first column */
    grid-row: 2 / 3; /* Starts below the image */
    color:black;
  }

  .para-2, .para-3 {
    grid-row: 1 / 2; /* These start in the first row */
    color:black;
  }

  .para-2 {
    grid-column: 2 / 3; /* Paragraph 2 in the second column */
    color:black;
  }

  .para-3 {
    grid-column: 3 / 4; /* Paragraph 3 in the third column */
    color:black;
  }

</style>
