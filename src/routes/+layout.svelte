<script>
	import '$lib/css/styles.css';
	import Footer from '$lib/widgets/Footer.svelte';
	import Header from '$lib/widgets/Header.svelte';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<Footer />
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		position: relative;
		overflow: hidden;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 2rem var(--padding-h);
		width: 100%;
		box-sizing: border-box;
	}
</style>
