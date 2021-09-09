<script>
    import Dropdown from '../Utility/Dropdown.svelte'
</script>

<Dropdown title="LambdaCalcEval">
    <slot>
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
    </slot>
</Dropdown>

<style>
    .fit {
        display: absolute;
        display: block;
        max-width: 100%;
        width: 100%;
        height: auto;
    }

</style>