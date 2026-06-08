<script>
	import favicon from '$lib/assets/logo.svg';

	let { children } = $props();
</script>

<svelte:head>
	<title>Antimony - Home</title> 
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
