<article class="currently-reading-card">
  <h1>Currently Reading</h1>

  <div class="book-info">
    <slot>
      <span class="title" />
    </slot>

    <slot>
      <span class="author" />
    </slot>

    <slot>
      <span class="began-reading" />
    </slot>
  </div>
</article>

<style>
  .currently-reading-card {
    width: 65%;
    margin: 4px auto;
    border: 1px solid black;
    border-radius: 15px;
    box-shadow: 2px 2px 8px rgba(0, 0, 0, 0.1);
    padding: 1em;
  }
  h1 {
    text-align: center;
    padding: 0 0 0.2em 0;
    margin: 0 0 1em 0;
    border-bottom: 1px solid green;
  }
</style>
