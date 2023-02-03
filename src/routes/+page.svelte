<script>
	import '../styles/all.css';
	import ProjectBlock from '../lib/ProjectBlock.svelte';
</script>

<div class="container project-container-spacing">
	<div class="content_container">
		<div class="block">
			<div class="body-1 intro ">
				Hello and welcome to my handcrafted internet space. I'm a designer and strategic thinker who
				enjoys collaborating, learning and laughing with other humans (live, laugh, love if you feel
				me). I'm always open to work with new people. Reach out and let's push things forward!
			</div>
			<div class="subhead">Recent Work</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Counter Situations</span>
				<span slot="year">Design and development for a funky web archive.</span>
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
					/></svelte:fragment
				>
				<span slot="visit" />
			</ProjectBlock>
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Trippin</span>
				<span slot="year">Design for a platform that connects travel, culture and creativity.</span>
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
					/></svelte:fragment
				>
				<span slot="visit" />
			</ProjectBlock>
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Recent Work</span>
				<span slot="year" />
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
			<div class="body-1  intro">
				I am also starting “Office Hours”. I way to meet and help designers or new companies
				navigate the industry. I’m happy to offer advice around process, careers, digital products,
				and strategy.
			</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Office Hours</span>
				<span slot="year">A personal project to connect through the internet.</span>
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
	<div class="content_container">
		<div class="block">
			<div class="subhead">Before</div>
			<div class="body-1 intro ">
				Hello and welcome to my handcrafted internet space. I'm a designer and strategic thinker who
				enjoys collaborating, learning and laughing with other humans (live, laugh, love if you feel
				me). I'm always open to work with new people. Reach out and let's push things forward!
			</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Recent Work</span>
				<span slot="year" />
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
					/></svelte:fragment
				>
				<span slot="visit" />
			</ProjectBlock>
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Recent Work</span>
				<span slot="year" />
				<svelte:fragment slot="image"
					><img
						class="thumbnail_image_selector"
						src="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
					/></svelte:fragment
				>
				<span slot="visit" />
			</ProjectBlock>
			<ProjectBlock>
				<!-- Using slots to reuse the components. The content structure for each block. -->
				<span slot="title">Recent Work</span>
				<span slot="year" />
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
				<span slot="year">A personal project to connect through the internet.</span>
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
		gap: calc(var(--spacing-unit));
		place-items: center;
	}

	.intro {
		margin-bottom: calc(var(--spacing-unit) * 4);
	}

	.thumbnail_image_selector {
		width: 100%;
		-webkit-box-shadow: 0px 12px 50px -22px rgba(0, 0, 0, 0.4);
		-moz-box-shadow: 0px 12px 50px -22px rgba(0, 0, 0, 0.4);
		box-shadow: 0px 12px 50px -22px rgba(0, 0, 0, 0.4);
	}
	.content_container {
		grid-column: col-start 2 / span 6;
		display: flex;
		flex-direction: column;
		gap: calc(var(--spacing-unit) * 4);
		padding-bottom: calc(var(--spacing-unit));
	}

	@media (min-width: 1600px) {
		.content_container {
			grid-column: col-start 2 / span 6;
		}
	}

	.project-container-spacing {
		margin-top: calc(var(--spacing-unit) * 8);
	}

	.project-container-spacing:first-child {
		margin-top: calc(var(--spacing-unit) * 8);
	}

	.subhead {
		top: 10rem;
		align-self: flex-start;
		/* this padding is to make it even to the project blcok underline */
		padding-bottom: calc(var(--spacing-unit) * 4);
	}
</style>
