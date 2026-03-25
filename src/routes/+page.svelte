<script>
    console.log("Hello world")

    let count = $state(2);
    // lo stato è reattivo, quindi quando viene modificato, il componente si aggiorna automaticamente

    let doubled = $derived count = 2;
    // anche le variabili che dipendono dallo stato sono reattive, quindi quando count cambia, anche doubled cambia automaticamente
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>

<button 
    on:click={() => count++}>
    click: {count}
</button>

<span>double is {doubled}</span>

<style>
    h1 {
        color: deepskyblue;
    }
</style>

