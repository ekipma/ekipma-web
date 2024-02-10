<script lang="ts">
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
		<enhanced:img
			class="phones"
			alt="ekipma payments"
			src="$lib/images/phones.avif?w=1280;640;400"
			sizes="(min-width:1920px) 1280px, (min-width:1080px) 640px, (min-width:768px) 400px"
		/>
		<!-- <enhanced:img
			class="phone-1"
			alt="ekipma payments"
			src="$lib/images/phone-0.avif?w=1280;640;400"
			sizes="(min-width:1920px) 1280px, (min-width:1080px) 640px, (min-width:768px) 400px"
		/> -->
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

	picture {
		display: contents;
	}

	.phones {
		height: 28vw;
		position: absolute;
		width: auto;
	}

	@media screen and (max-width: 800px) {
		section > * {
			flex: 0 0 100% !important;
			margin-bottom: 5rem;
		}

		.phones {
			height: 60vw;
		}
	}

	@media screen and (max-width: 750px) {
		.phones {
			height: 75vw;
		}
	}

	@media screen and (max-width: 500px) {
		.phones {
			height: 100vw;
		}
	}
</style>
