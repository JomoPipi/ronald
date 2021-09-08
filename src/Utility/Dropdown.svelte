
<script>
    export let title
	import { slide } from 'svelte/transition';

    let show = false
    function toggle() {
        show ^= true
    }
</script>

<li>
    <button class="btn btn-outline-primary" on:click={toggle}><h4>{title}</h4> <i class="arrow down"></i></button> 
    {#if show}
        <div class="container" transition:slide>
            <slot>Nothing here yet!</slot>
        </div>
    {/if}
</li>

<style>
    .container {
        text-align: center;
    }
    button {
        width: 90%;
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