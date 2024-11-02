<script>
  export let videoId = "9Mw0UERlzJY";
  export let videoId2 = "E60XAssGUgA";
  export let title = "Where The Edge of Me Meets Another";
</script>

<div class="container mx-auto p-4">
  <h1  style="color: black; font-size: 2em;"> Where the Edge of Me Meets Another</h1>

  <!-- Header -->
  <h1 class="text-3xl font-bold mb-4">{title}</h1>

  <!-- Video Embed -->
  <div class="video-container mb-4">
    <iframe
      width="100%"
      height="500"
      src={`https://www.youtube.com/embed/${videoId}`}
      title={title}
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    ></iframe>
  </div>

  <!-- Description Paragraphs -->
  <h2 class="text-lg mb-4 text-black">Where the Edge of Me Meets Another, 2024</h2>

  <p class="text-lg mb-4">
    This project is a fragment shader running in Touchdesigner that utilizes the <a href="https://cargocollective.com/sagejenson/physarum" target="_blank" style="color: blue; text-decoration: underline;">
    Physarum Algorithm from Artist Sage Jenson
    </a>.
    The piece is a realtime computed simulation of agents or ants, moving in cohesion with their neighbors, as well as being attracted 
    to people whom I have designated to be eaten. All of the photos are found, and people in the photos have no personal 
    connection.
  </p>

  <p class="text-lg mb-4">
    I arrived at this piece after experimenting with a shader implementation of Physarum with the goal of making a digital decomposition. In an attempt to visualize death as a dispersal of life-giving compounds. Below are remnants of prior animal-shaped pieces, made with a similar shader. 
  </p>

  <!-- Centered Second Video -->
  <div class="video-center mb-4">
    <iframe
      width="60%" 
      height="600"
      src={`https://www.youtube.com/embed/${videoId2}`}
      title={title}
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    ></iframe>
  </div>
  <div class="image-column">
    <img src="/physarum/rabbit_gray_1.webp" alt="Bio" class="bio-photo" style = "width:800px"/>
    <img src="/physarum/rabbit_gray_2.webp" alt="Bio" class="bio-photo" />
  </div>
</div>

<style>
  .video-container {
    position: relative;
    padding-bottom: 56.25%; /* 16:9 aspect ratio */
    height: 0;
    overflow: hidden;
  }
  .video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
  .video-center {
    display: flex;              /* Enable flexbox layout */
    justify-content: center;    /* Center the iframe horizontally */
    align-items: center;        /* Center the iframe vertically (optional) */
  }
  .image-column {
    display: flex;
    flex-direction: column; /* Arrange images in a column */
    align-items: center;    /* Center images in the column */
    gap: 10px;              /* Add space between images */
  }
</style>
