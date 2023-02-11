<script lang="ts">
	export let title, description, url, projectimage, imagealt;
</script>

<div class="thumbnail">
	<div class="thumbnail_image">
		<div class="thumbnail_image_image">
			<img src={projectimage} alt={imagealt} />
		</div>
	</div>
	<div class="thumbnail_caption">
		<div class="thumbnail_caption_text">
			<div class="thumbnail_caption_title ">{title}</div>
			<div class="thumbnail_caption_year">{description}</div>
		</div>
		<a href={url} target="blank">
			<div class="thumbnail_caption_link button-1">Visit</div>
		</a>
	</div>
</div>

<style>
	.thumbnail {
		width: 100%;
		display: flex;
		flex-direction: column;
		background-color: var(--gray-50);
		border-radius: 1rem;
	}

	.thumbnail_image {
		width: 100%;
	}

	.thumbnail_image img {
		width: 100%;
	}

	.thumbnail_image_image {
		padding: calc(var(--spacing-unit) * 3);
	}

	.thumbnail_caption {
		display: flex;
		flex-direction: row;
		justify-content: space-between;

		padding: 0 calc(var(--spacing-unit) * 3) calc(var(--spacing-unit) * 3);
		align-items: flex-end;
	}

	.thumbnail_caption_text {
		display: flex;
		flex-direction: column;
	}

	.thumbnail_caption_link {
		padding: 0.35rem 0.75rem;
		border-radius: 0.5rem;
		background-color: #e2e2e2;
	}
</style>
