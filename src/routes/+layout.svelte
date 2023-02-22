<script>
	import '../styles/all.css';
	import Header from '../lib/Header.svelte';
	import Footer from '../lib/Footer.svelte';
</script>

<Header />
<main>
	<slot />
</main>
<Footer />

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: flex-end;
		justify-content: center;
	}
</style>
