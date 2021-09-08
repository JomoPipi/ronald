<script>
    let show = false
    function toggle() {
        show ^= true
    }
</script>
<li>
    <h4>LambdaCalcEval <i class="arrow down"
        on:click={toggle}></i> </h4> 
    {#if show}
        <a target="_blank" href="https://lambdacalceval.ronaldmcorona.now.sh">
        LambdaCalcEval</a> is a <a target="_blank"
        href="https://en.wikipedia.org/wiki/Lambda_calculus"
        >lambda calculus</a> evaluator that runs on the browser.

        <br>

        I originally built it to make it easier to check my solutions to the exercises
        at the end of <a target="_blank"
        href="https://personal.utdallas.edu/~gupta/courses/apl/lambda.pdf"
        >this paper</a>.

        <ul>
            <li>
                It has an option to view the full reduction steps of each program
                (which can be tremendously long, even for small calculations).
            </li>
            <li>
                It has it’s own syntax highlighting and error messages.
            </li>
            <li>
                Below is a picture of <a target="_blank"
                href="https://lambdacalceval.ronaldmcorona.now.sh">
                LambdaCalcEval</a> with some code in it. It's an
                <code>isEven</code> function that works by successively applying the
                <code>not</code> function to <code>true</code>, <code>n</code> times.
            </li>
        </ul>
        <div>
            <img class="fit" alt="oops: broken" src="images/lambdacalceval.png">
        </div>
    {/if}
</li>

<style>
    .fit {
        display: absolute;
        display: block;
        max-width: 80%;
        width: 80%;
        height: auto;
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