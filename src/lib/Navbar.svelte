<script lang="ts">
    export let links = [
      { name: 'About Me', href: '#about-me' },
      { name: 'My Projects', href: '#projects' },
      { name: 'Experience', href: '#experience' }
    ];
  </script>
  
  <nav class="fixed top-0 left-0 w-full bg-gray-900 text-white shadow-md z-50">
    <div class="flex justify-between items-center p-6">
      <div class="font-bold text-xl">My Portfolio</div>
      <div class="space-x-6">
        {#each links as link}
          <a href={link.href} class="hover:text-gray-300">{link.name}</a>
        {/each}
      </div>
    </div>
  </nav>
  