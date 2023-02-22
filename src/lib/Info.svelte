<script>
</script>

<div class="info-container">
	<div>
		<div class="info-title">About</div>
		I'm a "digital" designer who enjoys helping people and teams navigate the fields of design & technology.
		It's fun to share what I've learned throughout my career with others as well as help them move their
		ideas forward. My favorite style of work is highly collaborative, open, honest and transparent.
	</div>
	<div>
		<div class="info-title">How I can Help</div>
		<div>My experience has helped me understand the importance of clear communication.</div>
	</div>
</div>

<style>
	.info-container {
		position: fixed;
		padding: var(--spacing-unit);
		overflow-y: scroll;
		left: -21%;
		background: white;
		border-right: 1px solid var(--color-primary);
		width: 20%;
		min-height: 100vh;
		top: 0;
		z-index: 4000;
		display: flex;
		flex-direction: column;
		gap: calc(var(--spacing-unit) * 2);
		-ms-wrap-flow: both;
		-ms-wrap-margin: 10px;
	}

	.info-title {
		display: inline-block;
		width: 20%;
		text-transform: uppercase;
	}

	.selected {
		left: -21%;
		background-color: #ff3e00;
		color: white;
	}
</style>
