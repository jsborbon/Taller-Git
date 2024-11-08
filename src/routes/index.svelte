<script lang="ts">
    import { goto } from '$app/navigation'; // Importa correctamente

    // Función para navegar a la página del contador
    const navigateToCounter = () => {
        goto('/counter'); // Asegúrate de que la ruta sea correcta
    };
</script>

<h1>Página de Inicio</h1>
<h1><a href="/counter">Counter</a></h1>
<button on:click={navigateToCounter}>Ir a Counter</button>