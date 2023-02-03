<div class="thumbnail">
	<div class="thumbnail_image">
		<!-- svelte-ignore a11y-missing-attribute -->
		<div class="thumbnail_image_image">
			<slot name="image" />
			<!-- <img src="https://karalevich.com/rho.webp" /> -->
		</div>
	</div>
	<div class="thumbnail_caption">
		<div class="thumbnail_caption_text">
			<div class="thumbnail_caption_title "><slot name="title" /></div>
			<div class="thumbnail_caption_year"><slot name="year" /></div>
		</div>
		<div class="thumbnail_caption_link button-1">
			<!-- conditional slot changing the link type based on the slot name -->
			<slot name="link" />
			{#if $$slots.visit}
				<div>Visit</div>
				<slot name="View" />
			{/if}
			{#if $$slots.view}
				<div>More</div>
				<slot name="More" />
			{/if}
		</div>
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
		padding: 0.5rem 0.75rem;
		border-radius: 0.5rem;
		color: white;
		background-color: var(--color-text);
	}
</style>
