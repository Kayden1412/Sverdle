<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<svelte:head>
    <title>Sverdle</title>
    <script async defer src="https://demo.tianji.msgbyte.com/tracker.js" data-website-id="cm03x03dzbxnpevvrpg8zyex4"></script>
</svelte:head>


<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
		<p>© 2023 - PRESENT</p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
