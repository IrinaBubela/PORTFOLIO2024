<script>
	import MainContent from "$lib/MainContent.svelte";
</script>

<svelte:head>
	<title>Irina Bubela</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<MainContent />

<style lang="scss">
	@import "../app.scss";
	:global(html) {
		background-color: $background;
	}
</style>
