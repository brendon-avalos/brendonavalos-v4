<script>
	import '../styles/all.css';
</script>

<header>
	<div class="name">
		<div class="name_name">Brendon Avalos</div>
	</div>
	<div class="links">
		<a href="/">Work</a>, <a href="">Info</a>, <a href="">Office Hours</a>
	</div>
</header>

<main>
	<slot />
</main>

<style>
	header {
		display: flex;
		justify-content: space-between;
		position: sticky;
		top: 1rem;
	}
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	header a {
		text-decoration: none;
	}

	.links {
		grid-column: col-start 7 / span 6;
	}
</style>
