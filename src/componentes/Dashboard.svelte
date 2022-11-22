<script>
    export let notes;
    import Note from "./Note.svelte";
</script>
<main>
    <div class="Dashboard">
        <div class="notes-container">
            {#each notes as {title, color, text}}
                <Note {title} {color} {text} />
            {/each}
        </div>
    </div>
</main>
<style>
    .Dashboard{
        width: 100%;
        padding: 20px;
        box-sizing: border-box;
    }
    .notes-container{
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        width: 100%;
        gap: 10px;
    }
</style>