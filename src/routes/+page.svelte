<script>
	import '../styles/all.css';
	import ProjectBlock from '../lib/ProjectBlock.svelte';
</script>

<div class="container">
	<div class="experience">Selected Work</div>
</div>

<div class="container project-container-spacing">
	<div class="current">Currently</div>
	<div class="content_container">
		<div class="block">
			<div class="body-1 intro">
				I am a designer at Fictive Kin. I contribute to both web & digital product projects for
				businesses large and small. I also manage projects and develop internal processes.
			</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Studio Carbon Negative</span>
				<span slot="year">2020</span>
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
					/></svelte:fragment
				>
				<span slot="visit" />
			</ProjectBlock>
		</div>

		<div class="block">
			<div class="body-1 intro">
				I am also starting “Office Hours”. I way to meet and help designers or new companies
				navigate the industry. I’m happy to offer advice around process, careers, digital products,
				and strategy.
			</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Office Hours</span>
				<span slot="year">2023</span>
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170997/original_74b379e51b31264aa66d5f435e4af2ca.jpg?1675321071?bc=0"
					/></svelte:fragment
				>
				<span slot="view" />
			</ProjectBlock>
		</div>
	</div>
</div>
<div class="container project-container-spacing">
	<div class="current">Before</div>
	<div class="content_container">
		<div class="block">
			<div class="body-1 intro">
				I am a designer at Fictive Kin. I contribute to both web & digital product projects for
				businesses large and small. I also manage projects and develop internal processes.
			</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Studio Carbon Negative</span>
				<span slot="year">2020</span>
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
					/></svelte:fragment
				>
				<span slot="visit" />
			</ProjectBlock>
		</div>

		<div class="block">
			<div class="body-1 intro">
				I am also starting “Office Hours”. I way to meet and help designers or new companies
				navigate the industry. I’m happy to offer advice around process, careers, digital products,
				and strategy.
			</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Office Hours</span>
				<span slot="year">2023</span>
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170997/original_74b379e51b31264aa66d5f435e4af2ca.jpg?1675321071?bc=0"
					/></svelte:fragment
				>
				<span slot="view" />
			</ProjectBlock>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Office Hours</span>
				<span slot="year">2023</span>
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170997/original_74b379e51b31264aa66d5f435e4af2ca.jpg?1675321071?bc=0"
					/></svelte:fragment
				>
				<span slot="view" />
			</ProjectBlock>
		</div>

		<div class="block">
			<div class="body-1 intro">
				I am also starting “Office Hours”. I way to meet and help designers or new companies
				navigate the industry. I’m happy to offer advice around process, careers, digital products,
				and strategy.
			</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Office Hours</span>
				<span slot="year">2023</span>
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170997/original_74b379e51b31264aa66d5f435e4af2ca.jpg?1675321071?bc=0"
					/></svelte:fragment
				>
				<span slot="view" />
			</ProjectBlock>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Office Hours</span>
				<span slot="year">2023</span>
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170997/original_74b379e51b31264aa66d5f435e4af2ca.jpg?1675321071?bc=0"
					/></svelte:fragment
				>
				<span slot="view" />
			</ProjectBlock>
		</div>
	</div>
</div>

<style>
	.block {
		display: grid;
		gap: calc(var(--spacing-unit) * 3);
	}

	.thumbnail_image_selector {
		width: 100%;
		-webkit-box-shadow: 0px 12px 50px -22px rgba(0, 0, 0, 0.4);
		-moz-box-shadow: 0px 12px 50px -22px rgba(0, 0, 0, 0.4);
		box-shadow: 0px 12px 50px -22px rgba(0, 0, 0, 0.4);
	}
	.content_container {
		grid-column: col-start 7 / span 6;
		display: flex;
		flex-direction: column;
		gap: calc(var(--spacing-unit) * 8);
	}

	@media (min-width: 1600px) {
		.content_container {
			grid-column: col-start 8 / span 5;
		}
	}

	.experience {
		justify-content: center;
		margin-top: calc(var(--spacing-unit) * 8 - 28px);
		margin-bottom: calc(var(--spacing-unit) * 8);
		grid-column: col-start 4 / span 2;
		position: sticky;
		align-self: flex-start;
		top: 1rem;
	}
	.current {
		position: sticky;
		top: 10rem;
		align-self: flex-start;
		/* this padding is to make it even to the project blcok underline */
		padding-bottom: calc(var(--font-size) / 8 + 1px);
	}
</style>
