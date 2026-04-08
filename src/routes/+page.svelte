<script>
import ClicksCounter from '$lib/componets/ClicksCounter.svelte';
let count = $state(0);
let doubled = $derived(count * 2);
    console.log('Hello World');
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>


<ClicksCounter bind:initialCount={count} />

<p>
    count from parent is {count}
</p>

<span>
doubled: {doubled}
</span>
<style>
	h1 {
		color: deepskyblue;
	}

    p {
        color: deeppink;
    }
</style>