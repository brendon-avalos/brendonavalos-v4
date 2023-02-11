<script>
	import '../styles/all.css';
</script>

<header>
	<div class="name">
		<div class="name_name uppercase">Brendon Avalos</div>
		<div class="name_description">Designer based in Los Angeles.</div>
	</div>
	<div class="links">
		<a href="/">Work</a>, <a href="">Info</a>, <a href="">Office Hours</a>
	</div>
</header>

<main>
	<slot />
</main>

<footer class="caption-1">
	<div class="footer-links">
		<div><a href="">Are.na</a></div>
		<div><a href="">E-mail</a></div>
		<div><a href="">LinkedIn</a></div>
	</div>
	<div class="copyright">
		<div>All rights reserved.</div>
		<div>© 2023 Brendon Avalos</div>
	</div>
</footer>

<style>
	header {
		display: flex;
		justify-content: flex-end;
		position: sticky;
		z-index: 1000;
		top: 1rem;
	}
	main {
		display: flex;
		flex-direction: column;
		align-items: flex-end;
		justify-content: center;
	}

	header a {
		text-decoration: none;
	}

	.links {
		grid-column: col-start 7 / span 6;
	}
	footer {
		display: flex;
		flex-direction: column;
		justify-content: flex-end;
		align-items: flex-end;
		gap: calc(var(--spacing-unit) / 2);
		min-height: calc(var(--spacing-unit) * 12);
	}

	.footer-links {
		display: flex;
		flex-direction: row;
		gap: 1rem;
	}

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
</style>
