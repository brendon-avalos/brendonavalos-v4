<script>
	import '../styles/all.css';
	import ProjectBlock from '../lib/ProjectBlock.svelte';
</script>

<div class="container project-container-spacing">
	<div class="content_container">
		<div class="block">
			<div class="body-1 intro ">
				Hello and welcome to my small corner of the internet. I'm a designer and strategic thinker
				who enjoys collaborating, learning and laughing with other humans (live, laugh, love if you
				feel me). Feel free to reach out and <span class="highlight"
					><a
						target="blank"
						href="https://www.youtube.com/watch?v=QOddpk8jOtU&ab_channel=TheStreets"
						>let's push things forward</a
					></span
				>.
			</div>
			<div class="subhead">Recent Work</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock
				title="Manhattan"
				description="Design for a platform that connects travel, culture and creativity."
				url="https:hydraulics.nyc"
				slide1="https://d2w9rnfcy7mm78.cloudfront.net/20332515/original_e7170818a5383a8e912379574b1040cf.jpg?1676097344?bc=0"
				slide2="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
				slide3="https://d2w9rnfcy7mm78.cloudfront.net/20187542/original_7bcd5db1f370aa4adc17fc1f925ba579.png?1675400351?bc=0"
			/>
			<ProjectBlock
				title="Manhattan"
				description="Design for a platform that connects travel, culture and creativity."
				url="https:hydraulics.nyc"
				slide1="https://d2w9rnfcy7mm78.cloudfront.net/20332515/original_e7170818a5383a8e912379574b1040cf.jpg?1676097344?bc=0"
				slide2="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
				slide3="https://d2w9rnfcy7mm78.cloudfront.net/20187542/original_7bcd5db1f370aa4adc17fc1f925ba579.png?1675400351?bc=0"
			/>
		</div>

		<div class="block">
			<div class="body-1  intro">
				I am also starting <span class="highlight"><a href="/">Office Hours</a></span>. A way to
				share what I've learned throughout my career to help designers and companies navigate the
				industry.
			</div>

			<ProjectBlock
				title="Manhattan"
				description="Design for a platform that connects travel, culture and creativity."
				url="https:hydraulics.nyc"
				slide1="https://d2w9rnfcy7mm78.cloudfront.net/20332515/original_e7170818a5383a8e912379574b1040cf.jpg?1676097344?bc=0"
				slide2="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
				slide3="https://d2w9rnfcy7mm78.cloudfront.net/20187542/original_7bcd5db1f370aa4adc17fc1f925ba579.png?1675400351?bc=0"
			/>
		</div>
	</div>
</div>

<div class="container project-container-spacing">
	<div class="content_container">
		<div class="block">
			<div class="subhead">Before</div>
			<div class="body-1 intro ">
				I also helped build a product design agency from the ground up with my friends at <span
					class="highlight"><a href="https://www.garden3d.net/">Garden3d</a></span
				>. I am proud that I helped foster a culture of trust and transparency within our team.
			</div>
			<!-- svelte-ignore a11y-missing-attribute -->
			<ProjectBlock
				title="Manhattan"
				description="Design for a platform that connects travel, culture and creativity."
				url="https:hydraulics.nyc"
				slide1="https://d2w9rnfcy7mm78.cloudfront.net/20332515/original_e7170818a5383a8e912379574b1040cf.jpg?1676097344?bc=0"
				slide2="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
				slide3="https://d2w9rnfcy7mm78.cloudfront.net/20187542/original_7bcd5db1f370aa4adc17fc1f925ba579.png?1675400351?bc=0"
			/>
			<ProjectBlock
				title="Manhattan"
				description="Design for a platform that connects travel, culture and creativity."
				url="https:hydraulics.nyc"
				slide1="https://d2w9rnfcy7mm78.cloudfront.net/20332515/original_e7170818a5383a8e912379574b1040cf.jpg?1676097344?bc=0"
				slide2="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
				slide3="https://d2w9rnfcy7mm78.cloudfront.net/20187542/original_7bcd5db1f370aa4adc17fc1f925ba579.png?1675400351?bc=0"
			/>
			<ProjectBlock
				title="Manhattan"
				description="Design for a platform that connects travel, culture and creativity."
				url="https:hydraulics.nyc"
				slidenumber="4"
				slide1="https://d2w9rnfcy7mm78.cloudfront.net/20332515/original_e7170818a5383a8e912379574b1040cf.jpg?1676097344?bc=0"
				slide2="https://d2w9rnfcy7mm78.cloudfront.net/20170975/original_7f953372f79f3bfb8e3cec4bb86ea4c9.png?1675320897?bc=0"
				slide3="https://d2w9rnfcy7mm78.cloudfront.net/20187542/original_7bcd5db1f370aa4adc17fc1f925ba579.png?1675400351?bc=0"
			/>
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
		border-radius: 0.5rem;
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
		margin-top: 30vh;
	}

	.subhead {
		top: 10rem;
		align-self: flex-start;
		/* this padding is to make it even to the project blcok underline */
		padding-bottom: calc(var(--spacing-unit) * 4);
	}
</style>
