<script lang="ts">
	import Slideshow from './Slideshow.svelte';

	export let title, description, url, slide1, slide2, slide3, year;
</script>

<div class="projectblock">
	<div class="thumbnail">
		<Slideshow {slide1} {slide2} {slide3} />
	</div>
	<div class="thumbnail_caption">
		<div class="thumbnail_caption_text">
			<div class="thumbnail_caption_header">
				<div class="thumbnail_caption_title uppercase">{title}</div>
				<div class="thumbnail_caption_year uppercase">{year}</div>
			</div>
			<div class="thumbnail_caption_year">
				{description}
				<a href={url} target="blank">
					<div class="thumbnail_caption_link ">Visit Website</div>
				</a>
			</div>
		</div>
	</div>
</div>

<style>
	.projectblock {
		width: 100%;
		min-width: 0;
		display: flex;
		flex-direction: column;
		gap: calc(var(--spacing-unit) * 0);
	}
	.thumbnail {
		display: flex;
		flex-direction: column;
		gap: calc(var(--spacing-unit) * 1);
		background: var(--gray-50);
		border: 1px solid var(--color-primary);
		padding: calc(var(--spacing-unit) * 3) calc(var(--spacing-unit) * 3)
			calc(var(--spacing-unit) * 3) calc(var(--spacing-unit) * 3);

		overflow: hidden;
	}

	.thumbnail_caption {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: baseline;
		padding: calc(var(--spacing-unit) * 2) calc(var(--spacing-unit) * 3)
			calc(var(--spacing-unit) * 0) calc(var(--spacing-unit) * 3);
	}
	.thumbnail_caption_header {
		display: flex;
		flex-direction: row;
		gap: calc(var(--spacing-unit) * 4);
		align-items: baseline;
	}

	.thumbnail_caption_title {
		text-indent: 4rem;
	}

	.thumbnail_caption_text {
		display: flex;
		flex-direction: column;
	}

	.thumbnail_caption_link {
		color: var(--highlight-color);
		display: inline;
	}
</style>
