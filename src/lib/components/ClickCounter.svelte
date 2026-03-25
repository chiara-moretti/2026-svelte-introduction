<script>
    console.log("Hello world")

    let count = $state(0);
    // lo stato è reattivo, quindi quando viene modificato, il componente si aggiorna automaticamente

    let doubled = $derived(count*2);
    // anche le variabili che dipendono dallo stato sono reattive, quindi quando count cambia, anche doubled cambia automaticamente

</script>

<h3>Clicks Counter</h3>

<button 
    on:click={() => count++}>
    click: {count}
</button>