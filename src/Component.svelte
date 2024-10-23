<script>
  import { getContext } from "svelte";

  const { styleable } = getContext("sdk");
  const component = getContext("component");
</script>

<style>
  .circle {
    height: 32px;
    width: 32px;
    background-color: green;
    border-radius: 50%;
  }
</style>

<div use:styleable={$component.styles} class="circle"></div>
