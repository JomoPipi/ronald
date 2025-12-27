<script>
  import Dropdown from "../Utility/Dropdown.svelte";
</script>

<Dropdown title="CodingPro" btnImgSrc="images/codingpro.png">
  <slot>
    <a
      target="_blank"
      href="https://codingpro.ronaldmcorona.vercel.app/problem?number=0"
    >
      CodingPro</a
    >
    is a tiny website meant to teach JavaScript to first time programmers. It's heavily
    inspired by
    <a target="_blank" href="https://codingbat.com">codingbat.com</a>. More
    questions still need to be added.
  </slot>
</Dropdown>

<style>
</style>
