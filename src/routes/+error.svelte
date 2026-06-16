<script>
  import { page } from '$app/stores';
  import Navbar from '$lib/navbar.svelte';
</script>

<Navbar />

<h1>{$page.status}</h1>

<p>{$page.error?.message}</p>

{#if $page.status === 404}
  <p>Aaaa! The page you're looking for doesn't exist.</p>
  <a href="/" style="color: #ADD8E6;">Go back home</a>
{/if}