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

			pagination: {
				el: '.swiper-pagination'
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
	</div>
	<div class="swiper-pagination" />
</div>

<style>
	.swiper {
		width: 100%;
		overflow: visible;
	}

	.swiper img {
		width: 100%;
		border: 1px solid var(--color-primary);
	}

	.swiper-slide {
		overflow: visible;
	}

	.swiper-wrapper {
		margin-bottom: calc(var(--spacing-unit) * 3);
		overflow: visible;
	}
</style>
