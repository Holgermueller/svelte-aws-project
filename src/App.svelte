<script>
  import Header from "./layout/Header.svelte";
  import CurrentlyReading from "./Components/CurrentlyReading.svelte";
  import Modal from "./shared/Modal.svelte";
  import Button from "./shared/Button.svelte";
  import BooksRead from "./Components/BooksRead.svelte";
  import Footer from "./layout/Footer.svelte";

  let showModal = false;

  let toggleModal = () => {
    showModal = !showModal;
  };
</script>

<Header />

<CurrentlyReading />

<Modal {showModal} on:click={toggleModal}>
  <h1>This is the modal</h1>
</Modal>

<Button on:click={toggleModal}>Add A Book</Button>

<BooksRead />

<Footer />
