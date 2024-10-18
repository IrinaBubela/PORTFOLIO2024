<script lang="ts">
	import Navbar from "$lib/Navbar.svelte";

	const links = [
    { name: 'Home', href: '/' },
    { name: 'About Me', href: '#about-me' },
    { name: 'Projects', href: '#projects' },
    { name: 'Experience', href: '#experience' }
  ];
</script>

<Navbar {links} />

<main class="flex flex-col items-center p-6 pt-20">
  <slot />
</main>


<style global>
	@import "../app.css";
</style>

