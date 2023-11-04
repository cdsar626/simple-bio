<script>
    export let title;
    export let description;
    export let url;

    function open_tab(url) {
        window.open(url, '_blank');
    }
</script>

<button class="card" on:click={open_tab(url)}>
    <h3>{title}</h3>
    <h5 class="word">{description}</h5>
</button>

<style>
    
    .card {
        border: 2px solid rgb(0, 0, 0);
        border-radius: 10px;
        will-change: filter;
        transition: filter 300ms;
    }

    .card:hover {
        filter: drop-shadow(0 0 2em #25e6ffd5);
    }
</style>