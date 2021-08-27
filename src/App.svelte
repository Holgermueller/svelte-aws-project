<script>
  import Header from "./layout/Header.svelte";
  import Modal from "./shared/Modal.svelte";
  import Button from "./shared/Button.svelte";
  import Footer from "./layout/Footer.svelte";

  let showModal = false;

  let toggleModal = () => {
    showModal = !showModal;
  };
</script>

<Header />

<Modal {showModal} on:click={toggleModal}>
  <h1>This is the modal</h1>
</Modal>

<Button on:click={toggleModal}>Add A Book</Button>

<Footer />
