<script lang="ts">
    import { goto } from "$app/navigation";
    import { fly } from 'svelte/transition';
</script>

<h1>Test nested layout</h1>

<button type="button" on:click={() => goto('/')}>Go Home</button>

<a href="/" out:fly={{ x: -6, delay: 200, duration: 300 }}>Link Home</a>

