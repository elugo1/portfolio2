<!-- src/lib/Card.svelte -->
<script>
    export let title = '';
    export let imageUrl = '';
    export let link = '';
  </script>
  
  <div class="card">
    <a href={link} class="block">
      <img src={imageUrl} alt={title} class="card-image opacity-70 transition-opacity duration-300 hover:opacity-100"/>

      <div class="card-title-overlay">
        <p class="card-title  text-white">{title}</p>
      </div>
    </a>
  </div>
  
  <style>
    .card {
      border: 1px solid #ddd;
      border-radius: 6px;
      overflow: hidden;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease;
      position: relative;
    }
  
    .card:hover {
      transform: scale(1.05);
    }
  
    .card-image {
      width: 100%;
      height: 20rem; /* Adjust as needed */
      object-fit: cover;
    }
  
    .card-title-overlay {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      background-color: rgba(0, 0, 0, 0.5); /* Semi-transparent background */
      color: white;
      padding: 0.5rem; /* Padding for readability */
      text-align: center;
    }
  
    .card-title {
      margin: 0;
      font-size: 1.25rem;
    }
  
    .card a {
      text-decoration: none;
      color: inherit;
      display: block;
    }
  </style>
  