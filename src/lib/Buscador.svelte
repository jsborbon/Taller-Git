<script>
    let search = ' ';
    const items = ['Pez', 'Pezz', 'Pezzz']

    function filterItems(){
        return items.filter(item => item.toLowerCase().includes(search.toLocaleLowerCase()))
    }
</script>


<div class="container">
    <p>Buscador</p>
    <input type="text" bind:value={search} placeholder="Buscar...">
    <ul>
        {#each items as item}
            <li>{item}</li>
        {/each}
    </ul>

    <ul>
        {#each filterItems() as item}
            <li>{item}</li>

        {/each}
    </ul>

</div>