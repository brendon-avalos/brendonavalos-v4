<script>
	import '../styles/all.css';
	import ProjectBlock from '../lib/ProjectBlock.svelte';
</script>

<div class="container project-container-spacing">
	<div class="content_container">
		<div class="body-1 intro text-indent">This is now an about route.</div>
	</div>
</div>

<style>
	.content_container {
		display: flex;
		flex-direction: column;
		gap: calc(var(--spacing-unit) * 2);
		padding-bottom: calc(var(--spacing-unit));
	}

	@media (min-width: 1600px) {
	}

	.project-container-spacing {
		margin-top: calc(var(--spacing-unit) * 8);
	}

	.project-container-spacing:first-child {
		margin-top: 30vh;
	}

	.subhead {
		display: flex;

		justify-content: center;
		align-content: center;
	}

	.subhead-text {
		text-transform: uppercase;
	}
</style>
