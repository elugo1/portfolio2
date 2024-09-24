<style>
  .grid-container {
    display: grid;
    grid-template-columns: repeat(1,1); /* Two columns of equal width */
    width: 100%; /* Full width of the page */
  }

  .grid-item {
    display: flex;
    justify-content: left;
    align-items: left;
    height:100%;
  }

  /* Ensure the image scales without cropping */
  img {
    max-width: 100%;
    height: auto;
    object-fit: contain; /* Ensures the whole image is shown without cropping */
  }

  /* Optional: Add a fixed height to the grid item to see how the image adjusts */
  .grid-item img {
    max-height: 100%; /* Set a reasonable height for the image */
  }
</style>

<div class="grid-container">
  <!-- Each ImgExp component is placed inside a grid item -->
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../plots/boquet_thumbnail.png', full: '../plots/boquet_full.png' }} />
  </div>
  
  <div class="grid-item">
    <p>This is my paragraph</p>
  </div>

  <!-- Add more grid items as needed -->
</div>

<script>
  import ImgExp from "../../../components/ImgExp.svelte";
</script>
