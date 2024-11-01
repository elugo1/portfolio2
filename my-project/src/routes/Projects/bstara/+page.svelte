<script>
    export let videoId = "7NlDTyZHXDE&t=3051s";
    export let videoId2 = "wJUzjAegH5Y&t=4023s";
    export let title = "Where The Edge of Me Meets Another";
  </script>
  
  <div class="container mx-auto p-4">
    <!-- Header -->
    <h1 class="text-3xl font-bold mb-4">{title}</h1>
  
    <!-- Video Embed -->
    <div class="video-container mb-4">
      <iframe
        width="100%"
        height="500"
        src="https://www.youtube.com/embed/7NlDTyZHXDE?si=u9jUBw2J3tdhhVvD"
        title={title}
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
    <h2 class="text-lg mb-4 text-black">STUDIO for Creative Inquiry B☆A, 2024</h2>
    <!-- Centered Second Video -->
    <div class="video-container mb-4">
        <iframe
          width="100%" 
          height="500"
          src="https://www.youtube.com/embed/wJUzjAegH5Y?si=ARRPXJPx58oN6q59"
          title={title}
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
    </div>
    <h2 class="text-lg mb-4 text-black">STUDIO for Creative Inquiry B☆A, 2023</h2>

    <!-- Description Paragraphs -->

  
    <p class="text-lg mb-4">
      B☆A is a student run project at Carnegie Mellon that originated in <a href="https://studioforcreativeinquiry.org/" target="_blank" style="color: blue; text-decoration: underline;">
        The STUDIO for Creative Inquiry 
        </a> in 2016. After the pandemic there had been a haitus where no students had taken up the tradition. In 2023, my friends and I decided to revive the student lecture series, a night of interdisciplinary fun where a dozen students get together to share their art, research, and projects that push the boundaries. In addition to being a presenter for two years of the event, I was lead-organizer for both events.  
.
    </p>
  
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
  