
<script>
    export let title

    let show = false
    function toggle() {
        show ^= true
    }
</script>

<li>
    <h4>{title} <button on:click={toggle}><i class="arrow down"></i></button> </h4> 
    {#if show}
        <slot>Nothing here yet!</slot>
    {/if}
</li>

<style>
    button {
        background: transparent;
        border-radius: 20px;
        margin: 1rem;
    }
    .arrow {
        border: solid white;
        border-width: 0 5px 5px 0;
        display: inline-block;
        padding: 5px;
        margin: 1rem;
    }

    .down {
        transform: rotate(45deg);
        -webkit-transform: rotate(45deg);
    }
</style>