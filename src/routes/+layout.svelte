<script>
	import '../styles/all.css';
</script>

<header class="text-1">
	<div class="name">Brendon Avalos</div>
	<div>
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
	}

	header a {
		text-decoration: none;
	}
</style>
