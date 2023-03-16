<script>
	export let slide1, slide2, slide3;
	// import Swiper bundle with all modules installed
	import Swiper from 'swiper/bundle';
	// register Swiper custom elements
	// import styles bundle
	// Republish

	import 'swiper/css/bundle';

	function initSwiper(node) {
		var swiper = new Swiper(node, {
			autoHeight: true,
			loop: true,
			spaceBetween: 300,
			pagination: {
				el: '.swiper-pagination'
			}
		});
	}
</script>

<div class="swiper" use:initSwiper>
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

	<div class="swiper-elements">
		<!-- If we need navigation buttons -->
		<!-- <div class="swiper-nav-container">
			<div class="swiper-nav-button swiper-button-prev" />
			<div class="swiper-nav-button swiper-button-next" />
		</div> -->
		<div class="swiper-pagination" />
	</div>
</div>

<style>
	.swiper {
		width: 100%;
		overflow: visible;
	}

	.swiper img {
		width: 100%;
		height: 100%;

		-webkit-box-shadow: 2px 22px 15px -11px rgba(0, 0, 0, 0.42);
		-moz-box-shadow: 2px 22px 15px -11px rgba(0, 0, 0, 0.42);
		box-shadow: 2px 22px 15px -11px rgba(0, 0, 0, 0.42);
	}

	.swiper-slide {
		overflow: visible;
	}

	.swiper-wrapper {
		overflow: visible;
	}

	.swiper-nav-button {
		width: 2rem;
		height: 2rem;
		border: 1px solid var(--color-primary);
		background-color: white;
	}
	.swiper-elements {
		margin-top: calc(var(--spacing-unit) * 3);
		height: 2rem;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
	}

	.swiper-nav-container {
		display: flex;
		justify-content: flex-start;
		align-items: center;
		gap: calc(var(--spacing-unit) / 2);
	}

	.swiper-button-prev {
		left: auto;
		right: auto;
		position: relative;
	}
	.swiper-button-next {
		left: auto;
		right: auto;
		position: relative;
	}

	.swiper-pagination {
		position: relative;
		width: auto;
		bottom: auto;
		top: auto;
	}
</style>
