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
		<div class="thumbnail_caption_link underline">
			<!-- conditional slot changing the link type based on the slot name -->
			<slot name="link" />
			{#if $$slots.visit}
				<div>Visit</div>
				<slot name="View" />
			{/if}
			{#if $$slots.view}
				<div>Learn More</div>
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
		gap: calc(var(--spacing-unit) * 2);
	}

	.thumbnail_image {
		width: 100%;
		background-color: var(--gray-50);
	}

	.thumbnail_image_image {
		padding: calc(var(--spacing-unit) * 3);
	}

	.thumbnail_caption {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: baseline;
	}

	.thumbnail_caption_text {
		display: flex;
		flex-direction: column;
	}
	.thumbnail_caption_title {
		text-indent: 3rem;
	}
	.thumbnail_caption_year {
	}
</style>
