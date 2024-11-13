<script>
    export let imgurl; // This is the image URL that will be passed in
    let showFullImage = false;
  
    function toggleImage() {
      showFullImage = !showFullImage;
    }
  </script>
  
  <style>
    .image-container {
      position: relative;
      width: 30%;
      /* height: 30%; */
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
      /* margin-left:20px; */
    }
  
    .image-container img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  
    .expand-icon {
      position: absolute;
      top: 10px;
      right: 10px;
      background: rgba(0, 0, 0, 0.5);
      color: white;
      padding: 5px;
      border-radius: 50%;
      cursor: pointer;
      display: flex;
      justify-content: center;
      align-items: center;
      width: 30px;
      height: 30px;
      border: none;
      opacity: 0; /* Initially hidden */
      pointer-events: auto; /* Ensure the button is clickable */
      transition: opacity 0.3s ease; /* Smooth fade-in */
    }
  
    .image-container:hover .expand-icon {
      opacity: 1; /* Show icon on hover */
    }
  
    .expand-icon i {
      font-size: 16px;
    }
  
    .modal {
      display: flex;
      justify-content: center;
      align-items: center;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.8);
      z-index: 1000;
    }
  
    .modal img {
      max-width: 70%;
      max-height: 70%;
    }
  </style>
  
  <div class="image-container">
    <img src={imgurl.thumbnail} alt="Thumbnail" />
    <button
      class="expand-icon"
      on:click={toggleImage}
      on:keydown={(e) => (e.key === 'Enter' || e.key === ' ') && toggleImage()}
      aria-label="Expand Image"
    >
      <i class="fas fa-search"></i>
    </button>
  </div>
  
  {#if showFullImage}
    <div class="modal" on:click={toggleImage} tabindex="0">
      <img src={imgurl.full} alt="Full" />
    </div>
  {/if}
  