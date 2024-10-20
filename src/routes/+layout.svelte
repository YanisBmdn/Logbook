<script>
	import './app.css';
	import './reset.css';
</script>

<div class="app">
	<main>
		<slot />
	</main>
	<footer>Made with SvelteKit</footer>
</div>

<style>
	footer {
		text-align: center;
	}
	.app {
        display: flex;
        flex-direction: column;
	}
    main{
        flex:1;
    }
</style>
