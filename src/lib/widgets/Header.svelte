<script>
	import logo from '$lib/images/app-logo.svg';
</script>

<header>
	<div class="corner">
		<a href="https://ekipma.ir">
			<img src={logo} alt="ekipma logo" />
		</a>
	</div>
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		padding: 2rem var(--padding-h);
		box-sizing: border-box;
	}

	.corner {
		height: 3em;
		width: auto;
	}

	.corner > a {
		display: contents;
	}

	.corner img {
		height: 100%;
		object-fit: contain;
	}
</style>
