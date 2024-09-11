<!-- src/lib/Card.svelte -->
<script>
    export let title = '';
    export let imageUrl = '';
    export let link = '';
  </script>
  
  <div class="card">
    <a href={link} class="block">
      <img src={imageUrl} alt={title} class="card-image"/>
      <!-- <div class="card-content"> -->
        <p class="card-title">{title}</p>
      <!-- </div> -->
    </a>
  </div>
  
  <style>
    .card {
      border: 1px solid #ddd;
      border-radius: 2px;
      overflow: hidden;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      transition: transform 0.2s ease;
    }
  
    .card:hover {
      transform: scale(1.05);
    }
  
    .card-image {
      width: 100%;
      height: 200px; /* Adjust as needed */
      object-fit: cover ;
    }
    .card-content {
    /* position: absolute; */
    /* bottom: 0; */
    /* left: 0; */
    /* width: 100%; */
    background-color: rgba(0, 0, 0, 0.25); /* Semi-transparent background */
    /* color: white; */
    padding: 1rem;
    box-sizing: border-box; /* Ensure padding doesn't affect width */
    text-align: center; /* Center text */
    z-index: 10; /* Ensure it appears above the image */
  }
    .card-title {
      padding: 1rem;
      background-color: rgba(0, 0, 0, 0.5);
      font-size: 1.25rem;
      /* color: #333; */
      text-align: center;
    }
  
    .card a {
      text-decoration: none;
      color: inherit;
    }
  </style>
  