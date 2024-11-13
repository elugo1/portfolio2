

<div class="grid-container">
  <!-- Each ImgExp component is placed inside a grid item -->
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../plots/boquet_thumbnail.png', full: '../plots/boquet_full.png' }} />
    <ImgExp imgurl={{ thumbnail: '../plots/l-system-full.png', full: '../plots/l-system-full.png' }} />
  </div>
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../plots/shape_tunnel4.png', full: '../plots/shape_tunnel4.png' }} />

  </div>
  <div class="grid-item">
    <p>This is my paragraph</p>
  </div>

  <!-- Add more grid items as needed -->
</div>

<script>
  import ImgExp from "../../../components/ImgExpPlot.svelte";
</script>
<style>
  .grid-container {
    display: grid;
    grid-template-columns: repeat(2,2); /* Two columns of equal width */
    grid-template-rows: repeat(2,1);
    width: 100%; /* Full width of the page */
  }

  .grid-item {
    display: flex;
    justify-content: center;
    align-items: center;
    gap:20px;

  }


  /* Optional: Add a fixed height to the grid item to see how the image adjusts */

</style>