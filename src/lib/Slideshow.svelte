<script>
	export let slide1, slide2, slide3;
	// import Swiper bundle with all modules installed
	import Swiper from 'swiper/bundle';

	// import styles bundle
	import 'swiper/css/bundle';
	import { onMount } from 'svelte';

	onMount(() => {
		const swiper = new Swiper('.swiper', {
			// Optional parameters
			autoHeight: true,
			spaceBetween: 300,

			// If we need pagination
			pagination: {
				el: '.swiper-pagination'
			},

			// Navigation arrows
			navigation: {
				nextEl: '.swiper-button-next',
				prevEl: '.swiper-button-prev'
			}
		});
		console.log(swiper.activeIndex);
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
	</div>
	<div class="swiper-pagination" />
	<!-- If we need navigation buttons -->
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

		-webkit-box-shadow: 2px 22px 15px -11px rgba(0, 0, 0, 0.42);
		-moz-box-shadow: 2px 22px 15px -11px rgba(0, 0, 0, 0.42);
		box-shadow: 2px 22px 15px -11px rgba(0, 0, 0, 0.42);
	}

	.swiper-slide {
		overflow: visible;
	}

	.swiper-wrapper {
		margin-bottom: calc(var(--spacing-unit) * 3);
		overflow: visible;
	}
</style>
