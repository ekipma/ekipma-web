<script lang="ts">
	import github from '$lib/images/github.svg';
</script>

<footer>
	<nav class="row">
		<a href="/">قوانین</a>
		<a href="/">حریم خصوصی</a>
		<a href="/">ارتباط با ما</a>
		<a href="https://github.com/ekipma">گیت هاب</a>
		<div class="spacer" />
		<a href="https://github.com">
			<img alt="github" src={github} class="icon-image" />
		</a>
	</nav>
</footer>

<style>
	footer {
		padding: 1rem 3rem;
	}

	footer nav {
		gap: 2.5em;
		align-items: center;
		justify-content: space-between;
	}

	.icon-image {
		opacity: 0.7;
	}
</style>
