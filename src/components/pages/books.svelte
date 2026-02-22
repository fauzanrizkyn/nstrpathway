<script>
    import Getbooks from "./getbooks.svelte";
</script>
<div id="books">
    <h2>Koleksi Buku</h2>
    <div class="booksCarousel">
        <Getbooks />
    </div>


</div>

<style>
    #books {
        padding: 2% 0 2% 0;
        width: fit-content;
        text-align: center;
    }
    .booksCarousel {
        margin-top: 2%;
        display: grid;
        grid-template-columns: repeat(6, 1fr);
        gap: 20px;
        overflow-x: scroll;
    }
    
</style>