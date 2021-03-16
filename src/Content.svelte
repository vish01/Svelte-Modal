<script>
  import { getContext } from "svelte";
  const { open } = getContext("simple-modal");

  export let buttonText, popupContent, style;
  const showPopup = () => open(popupContent);

</script>
<button on:click={showPopup} {style}>{buttonText}</button>