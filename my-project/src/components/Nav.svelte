<script>
  import { page } from '$app/stores';
  let message = "";

  function copyEmail() {
    const email = "emmanuel.lugo1007@gmail.com"; // Replace with your actual email
    navigator.clipboard.writeText(email).then(() => {
      message = "Email copied to clipboard!";
      setTimeout(() => {
        message = "";
      }, 3000); // Message disappears after 3 seconds
    }).catch(err => {
      console.error('Failed to copy: ', err);
    });
  }
</script>

<nav class="bg-neutral-000 p-4 sticky flex justify-between items-center">
  <ul class="flex space-x-4">
    <li>
      <a 
        href="/" 
        class={`relative text-black text-2xl hover:text-gray-400 ${$page.url.pathname === '/Projects' ? 'text-blue-500' : ''}`}
      >
        Projects
        {#if $page.url.pathname === '/Projects'}
          <span class="absolute block w-full h-0.5 bg-blue-500 bottom-0 left-0"></span>
        {/if}
      </a>
    </li>
    <li>
      <a 
        href="/Info" 
        class={`relative text-black text-2xl hover:text-gray-400 ${$page.url.pathname === '/Info' ? 'text-blue-500' : ''}`}
      >
        Info
        {#if $page.url.pathname === '/Info'}
          <span class="absolute block w-full h-0.5 bg-blue-500 bottom-0 left-0"></span>
        {/if}
      </a>
    </li>
    <li class="relative">
      <!-- Contact button now wrapped in a relative container for positioning -->
      <button 
        on:click={copyEmail} 
        class={`relative text-black text-2xl hover:text-gray-400 ${$page.url.pathname === '/Contact' ? 'text-blue-500' : ''}`}
      >
        Contact
        {#if $page.url.pathname === '/Contact'}
          <span class="absolute block w-full h-0.5 bg-blue-500 bottom-0 left-0"></span>
        {/if}
      </button>
      <!-- Position the message absolutely next to the Contact button -->
      {#if message}
        <div class="absolute top-full left-0 mt-1 whitespace-nowrap text-green-600 bg-gray-100  p-1 rounded">
          {message}
        </div>
      {/if}
    </li>
  </ul>

  <!-- External icons on the right -->
  <div class="flex space-x-4">
    <a href="https://github.com/elugo1" target="_blank" rel="noopener noreferrer" class="text-black hover:text-gray-400">
      <i class="fab fa-github text-4xl"></i>
    </a>
    <a href="https://instagram.com/shrugbread" target="_blank" rel="noopener noreferrer" class="text-black hover:text-gray-400">
      <i class="fab fa-instagram text-4xl"></i>
    </a>
    <a href="https://www.linkedin.com/in/emlugo-art/" target="_blank" rel="noopener noreferrer" class="text-black hover:text-gray-400">
      <i class="fab fa-linkedin text-4xl"></i>
    </a>
  </div>
</nav>
