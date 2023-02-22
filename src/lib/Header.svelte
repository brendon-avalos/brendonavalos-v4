<header>
	<div class="name">
		<div class="name_name uppercase">Brendon Avalos</div>
		<div class="name_description">Designer based in Los Angeles.</div>
	</div>
	<div class="links">
		<a href="/">Work</a>,
		<button on:click>Info</button>
		<a href="">Office Hours</a>
	</div>
</header>

<style>
	.copyright {
		display: flex;
		flex-direction: row;
		gap: 1rem;
	}

	.name {
		position: fixed;
		bottom: 1rem;
		left: 1.5rem;
	}

	.name_name {
		text-indent: 2rem;
	}

	header {
		display: flex;
		justify-content: flex-end;
		position: sticky;
		z-index: 1000;
		top: 1rem;
	}

	header a {
		color: var(--color-primary);
	}
</style>
