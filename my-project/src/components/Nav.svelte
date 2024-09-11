<script>
  import { page } from '$app/stores';
</script>

<nav class="bg-neutral-000 p-4">
  <ul class="flex space-x-4  ">
    <li>
      <a 
        href="/Projects" 
        class={`relative text-black hover:text-gray-400 ${$page.url.pathname === '/Projects' ? 'text-blue-500' : ''}`}
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
        class={`relative text-black hover:text-gray-400 ${$page.url.pathname === '/Info' ? 'text-blue-500' : ''}`}
      >
        Info
        {#if $page.url.pathname === '/Info'}
          <span class="absolute block w-full h-0.5 bg-blue-500 bottom-0 left-0"></span>
        {/if}
      </a>
    </li>
    <li>
      <a 
        href="/Contact" 
        class={`relative text-black hover:text-gray-400 ${$page.url.pathname === '/Contact' ? 'text-blue-500' : ''}`}
      >
        Contact
        {#if $page.url.pathname === '/Contact'}
          <span class="absolute block w-full h-0.5 bg-blue-500 bottom-0 left-0"></span>
        {/if}
      </a>
    </li>
  </ul>
</nav>
