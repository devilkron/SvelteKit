<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>
		<span class="welcome">
			<picture>
				<source srcset={welcome} type="image/webp" />
				<img src={welcome_fallback} alt="Welcome" />
			</picture>
		</span>

	</h1>

	<div class="flex flex-row">
			<div class="font-bold">ชื่อ - นามสกุล:</div>
			<div class="text-sky-500">นายฉลองราช ภูครองนาค</div>
	</div>

	<div class="flex flex-row">
		<div class="font-bold">Facebook: </div>
		<div class="text-sky-500 hover:text-purple-500"><a target="_blank" href="https://www.facebook.com/CP.KornEiEi40/">Chalongrach Phukhongnak</a></div>
	</div>
	<div class="flex flex-row">
		<div class="font-bold">Instagram: </div>
		<div class="text-sky-500"><a href="/">kkorn_ii</a></div>
	</div>
	

	<!-- <Counter /> -->
</section>

<!-- <style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style> -->
