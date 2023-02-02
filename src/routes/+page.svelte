<script>
	import '../styles/all.css';
</script>

<div class="container">
	<div class="experience">Experience</div>
</div>

<div class="container">
	<div class="current">Currently</div>
	<div class="body-1 narrative">
		I am a designer at Fictive Kin. I contribute to both web & digital product projects for
		businesses large and small. I also manage projects and develop internal processes.
	</div>
</div>

<style>
	.experience {
		justify-content: center;
		align-items: center;
		margin-top: calc(var(--spacing-unit) * 5);
		margin-bottom: calc(var(--spacing-unit) * 5);
		grid-column: col-start 4 / span 2;
	}
	.current {
		grid-column: col-start 1 / span 2;
	}

	.narrative {
		grid-column: col-start 7 / span 6;
	}

	@media (min-width: 1600px) {
		.narrative {
			grid-column: col-start 9 / span 4;
		}
	}
</style>
