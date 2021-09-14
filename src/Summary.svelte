<script>
    let show = true
    function toggle() {
        show ^= true
    }
</script>

<h3> Summary 
    <!-- <i class="arrow down" on:click={toggle}></i> -->
</h3> 
{#if show}
    <p>
        Hi, I'm Ronald!
        <br>
        I started learning programming in 2017, and I really enjoy it.
        <!-- <br>
        Here is some proof that he considers me a dependable person.
        <br>
        <video width="320" height="240" controls loop="true">
            <source src="images/ollie.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video> -->
    </p>
{/if}

<!-- <style>
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

</style> -->