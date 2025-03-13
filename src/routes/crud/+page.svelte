<script>
  let items = [];
  let newItem = '';

  function addItem() {
    if (newItem) {
      items = [...items, newItem];
      newItem = '';
    }
  }

  function removeItem(index) {
    items = items.filter((_, i) => i !== index);
  }
</script>

<main>
  <p>This task involves Create, Read, Update, and Delete operations on a list of items.</p>
  <h1>CRUD</h1>
  <input type="text" bind:value={newItem} />
  <button on:click={addItem}>Add</button>
  <ul>
    {#each items as item, index}
      <li>
        {item} <button on:click={() => removeItem(index)}>Remove</button>
      </li>
    {/each}
  </ul>
</main>
