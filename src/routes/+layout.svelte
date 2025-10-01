<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
	import { base } from '$app/paths';

	let { children } = $props();
</script>

<nav>
	<a href="{base}/traningspass">Träningspass</a>
</nav>
<hr>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children?.()}

<style>
	a {
		color: black;
	}

	a:hover {
		background-color: aquamarine;
	}
</style>