<script>
	import { onMount } from 'svelte';

	// import Swiper bundle with all modules installed
	import Swiper from 'swiper/bundle';

	// import styles bundle
	import 'swiper/css/bundle';

	export let slide1, slide2, slide3;

	onMount(() => {
		const swiper = new Swiper('.swiper', {
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
	});
</script>

<div class="swiper">
	<!-- Additional required wrapper -->
	<div class="swiper-wrapper">
		<!-- Slides -->
		<div class="swiper-slide">{slide1}</div>
		<div class="swiper-slide">{slide2}</div>
		<div class="swiper-slide">{slide3}</div>
		...
	</div>
	<!-- If we need pagination -->
	<div class="swiper-pagination" />

	<!-- If we need navigation buttons -->
	<div class="swiper-button-prev" />
	<div class="swiper-button-next" />

	<!-- If we need scrollbar -->
	<div class="swiper-scrollbar" />
</div>

<style>
	.swiper {
		width: 100%;
	}
</style>
