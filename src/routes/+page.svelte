<script>
    console.log("Hello world")

    let count = $state(0);
    // lo stato è reattivo, quindi quando viene modificato, il componente si aggiorna automaticamente

    let doubled = $derived(count*2);
    // anche le variabili che dipendono dallo stato sono reattive, quindi quando count cambia, anche doubled cambia automaticamente

    import ClickCounter from "$lib/components/ClickCounter.svelte";
    import ProgressiveSum from "$lib/components/ProgressiveSum.svelte";
    // è possibile importare componenti da altri file e usarli come tag HTML

</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>

<ClickCounter />
<ProgressiveSum />

<style>
    h1 {
        color: deepskyblue;
    }
</style>

