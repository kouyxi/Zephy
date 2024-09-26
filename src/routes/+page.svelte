<script>
	function open() {
		alert('hello world');
	}
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<button on:click={open}>Open</button>

<style>
	button {
		background: var(--feat);
		color: white;
	}
</style>
