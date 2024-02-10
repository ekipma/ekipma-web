<script lang="ts">
	import phone0 from '$lib/images/phone-0.avif?enhanced';
	import android from '$lib/images/android.svg';
	import apple from '$lib/images/apple.svg';
</script>

<svelte:head>
	<title
		>اکیپــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــما</title
	>
	<meta name="description" content="برای اکیپ ما" />
</svelte:head>

<section>
	<div class="content">
		<h1>اکیپما اینجاست تا برای اکیپتون کلی کارای باحال انجام بده</h1>
		<div class="row gap-1">
			<a class="btn" href="https://cdn.ekipma.ir/ekipma.apk">
				<img alt="android" src={android} class="icon-image-sm" />
				<span>دانلود اندروید</span>
			</a>
			<button>
				<img alt="android" src={apple} class="icon-image-sm" />
				<span>دانلود آیفون</span>
			</button>
		</div>
	</div>
	<div class="mockup">
		<div class="ambient-light" />
		<enhanced:img class="phone-0" alt="ekipma payments" src={phone0} />
		<enhanced:img class="phone-1" alt="ekipma payments" src={phone0} />
	</div>
</section>

<style>
	section {
		flex: 1;
		display: flex;
		flex-direction: row;
		flex-wrap: wrap-reverse;
		justify-content: space-between;
		align-items: center;

		container-type: inline-size;
		container: home-section;
	}

	.content {
		flex: 0 0 50%;
		display: flex;
		flex-direction: column;
		gap: 2rem;
		max-width: 30rem;
	}

	.mockup {
		flex: 0 0 40%;
		display: flex;
		align-items: center;
		justify-content: center;
		min-height: 25rem;
	}

	.ambient-light {
		position: absolute;
		z-index: 0;
		height: 60rem;
		width: 60rem;
		background: radial-gradient(circle at center, var(--color-primary) 0, #fff0 50%);
		border-radius: 50%;
		transform: translate(-0rem, -5rem);
		opacity: 0.18;
	}

	.mockup img {
		height: 28vw;
	}

	img.phone-0 {
		position: absolute;
		width: auto;
		transform: translateX(10vw) scale(0.75);
	}

	img.phone-1 {
		position: absolute;
		width: auto;
	}

	@media screen and (max-width: 800px) {
		section > * {
			flex: 0 0 100% !important;
			margin-bottom: 5rem;
		}

		.mockup img {
			height: 60vw;
		}

		img.phone-0 {
			display: none;
		}
	}

	@media screen and (max-width: 750px) {
		.mockup img {
			height: 75vw;
		}
	}

	@media screen and (max-width: 500px) {
		.mockup img {
			height: 100vw;
		}
	}
</style>
