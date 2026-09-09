<script lang="ts">
	import './layout.css';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href="/logo-navbar.jpeg" /></svelte:head>
{@render children()}
