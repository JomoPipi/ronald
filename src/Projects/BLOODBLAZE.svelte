<script>
    import Dropdown from '../Utility/Dropdown.svelte'
</script>

<Dropdown
    title="BLOOD BLAZE"
    btnImgSrc="images/bloodblaze.png">
    <slot>
        <a target="_blank" href="https://bloodblaze.io">
        BLOOD BLAZE</a> is a 2D top-down fast-paced multiplayer shooter game.
        It works on mobile and desktop browsers. Shoot your friends in the face and enjoy.
        <img class="fit" alt="oops: broken" src="images/bloodblaze3.png">
        <img class="fit" alt="oops: broken" src="images/bloodblaze2.png">
    </slot>
</Dropdown>

<style>
    .fit {
        display: absolute;
        display: block;
        max-width: 80%;
        width: 80%;
        height: auto;
        margin-bottom: 1em;
    }
</style>