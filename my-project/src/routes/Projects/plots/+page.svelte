

<div class="grid-container">
  <div class="grid-item">
    <p text-lg mb-4 style="max-width: 60%; padding-bottom: 20px;"> A small showing of generated pen plots and SVGs from Touchdesigner and Houdini. The plots are rubbed into the page with a stylus depressed onto carbon-transfer paper.</p>

  </div>
  <!-- Each ImgExp component is placed inide a grid item -->
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../plots/boquet_thumbnail.png', full: '../plots/boquet_full.png' }} />
  </div>
  <div class ="grid-item">
  <ImgExp imgurl={{ thumbnail: '../plots/l-system-full.png', full: '../plots/l-system-full.png' }} />
</div>
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../plots/shape_tunnel4.png', full: '../plots/shape_tunnel4.png' }} />
  </div>
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../plots/boquet_scan.jpeg', full: '../plots/boquet_scan.jpeg' }} />
  </div>
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../thumbnail_images/double_wreath_thumbnail.png', full: '../plots/double_wreath.png' }} />
  </div>
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../plots/chair_plot.png', full: '../plots/chair_plot.png' }} />
  </div>
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../thumbnail_images/interdigit_thumbail.png', full: '../plots/interdigit.png' }} />
  </div>
  <div class="grid-item">
    <ImgExp imgurl={{ thumbnail: '../plots/deer_walking_1.png', full: '../plots/deer_walking_1.png' }} />
  </div>
  <div class ="grid-item">
  <iframe width="40%" height="315" src="https://www.youtube.com/embed/p4_S6nR6Rfo?si=pQUzCeWXKD6_k3Nu" loading = "lazy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
    padding-bottom:10px;

  }


  /* Optional: Add a fixed height to the grid item to see how the image adjusts */

</style>