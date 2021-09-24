
<script>
    export let title
    export let btnImgSrc
	import { slide } from 'svelte/transition';

    let show = false
    function toggle() {
        show ^= true
    }
</script>

<div class="showing">
    <button class="btn btn-outline-primary"
        on:click={toggle}>
        {title}
        <img class="pic" alt="nunisynth" src={btnImgSrc}>
        <i class="arrow down"></i>
    
    </button> 
    {#if show}
        <div class="container" transition:slide>
            <slot>Nothing here yet!</slot>
        </div>
    {/if}
</div>

<style>
    button {
        text-align: left;
        width: 100%;
        /* height: 80px; */
        margin: auto;
        margin-bottom: 1rem;
        font-size: 2rem;
    }
    .arrow {
        float: right;
        border: solid white;
        border-width: 0 5px 5px 0;
        padding: 5px;
        margin: 0.5rem;
    }
    .down {
        transform: rotate(45deg);
        -webkit-transform: rotate(45deg);
    }
    .showing {
        display: sticky;
        top: 0;
    }
    .pic {
        display: block;
        width: 50%;
        height: auto;
        margin: auto;
    }
</style>