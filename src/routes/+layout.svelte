<script>
	import favicon from '/logo.svg';
	import '$lib/assets/style.css';

	let { children } = $props();
</script>

<svelte:head>
	<title>Antimony - Home</title> 
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
