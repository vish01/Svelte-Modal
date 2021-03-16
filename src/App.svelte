<script>
  import Content from "./Content.svelte";
	import PopupContent from "./PopupContent.svelte";
  import Modal from "./Modal.svelte";
  import { writable } from "svelte/store";
  export const modal = writable(null);
</script>

<Modal show={$modal}>
  <Content
    buttonText="Click Me"
    popupContent={PopupContent}
    style="color: red;" />
</Modal>
