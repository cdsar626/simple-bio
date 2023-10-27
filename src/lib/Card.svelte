<script>
    export let title;
    export let description;
    export let url;

    let clazz = '';
    export {clazz as class};
</script>

<button class="card {clazz}" >
    <h3>{title}</h3>
    <h5>{description}</h5>
</button>

<style>
    .span2 {
        grid-column-end: span 2;
    }
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