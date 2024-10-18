<script>
	import "../app.scss";
	import Navbar from "$lib/Navbar.svelte";

	const links = [
		{ name: "Home", href: "/" },
		{ name: "About Me", href: "#about-me" },
		{ name: "Projects", href: "#projects" },
		{ name: "Experience", href: "#experience" },
	];
</script>

<Navbar {links}></Navbar>

<main class="flex flex-col items-center p-6 pt-20">
	<slot></slot>
</main>

<style>
	@import "../app.scss";
</style>
