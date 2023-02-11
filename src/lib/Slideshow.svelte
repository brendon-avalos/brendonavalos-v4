<script>
	import { onMount } from 'svelte';

	// import Swiper bundle with all modules installed
	import Swiper from 'swiper/bundle';

	// import styles bundle
	import 'swiper/css/bundle';

	export let slide1, slide2, slide3;

	onMount(() => {
		const swiper = new Swiper('.swiper', {
			spaceBetween: 300,
			autoHeight: true,
			centeredSlides: true,
			// If we need pagination
			navigation: {
				nextEl: '.swiper-button-next',
				prevEl: '.swiper-button-prev'
			},
			hashNavigation: {
				watchState: true
			},
			pagination: {
				el: '.swiper-pagination',
				clickable: true
			}
		});
		swiper.loopDestroy();
		swiper.loopCreate();
	});
</script>

<div class="swiper">
	<!-- Additional required wrapper -->
	<div class="swiper-wrapper">
		<!-- Slides -->
		<!-- svelte-ignore a11y-missing-attribute -->
		<div class="swiper-slide"><img src={slide1} /></div>
		<!-- svelte-ignore a11y-missing-attribute -->
		<div class="swiper-slide"><img src={slide2} /></div>
		<!-- svelte-ignore a11y-missing-attribute -->
		<div class="swiper-slide"><img src={slide3} /></div>
		...
	</div>
	<div class="swiper-pagination" />

	<!-- If we need pagination -->
	<div class="swiper-button-prev" />
	<div class="swiper-button-next" />
</div>

<style>
	.swiper {
		width: 100%;
		overflow: visible;
	}

	.swiper img {
		width: 100%;
		box-shadow: 0 12px 50px -22px #0006;
		border-radius: 0.5rem;
	}
</style>
