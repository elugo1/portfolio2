<script>
    import "../app.css";
    import Nav from '../components/Nav.svelte';
    import Header from '../components/Header.svelte';
  </script>
  <!-- <div class = "relative flex flex-col max-w-[1400px] mx-auto w-full text-small 
  sm:text-base min-h-screen">

  </div> -->
  <Header/>
  <Nav />
  <slot />
  