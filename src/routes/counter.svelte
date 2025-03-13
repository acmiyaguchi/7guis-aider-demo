<script>
  let count = 0;

  function increment() {
    count += 1;
  }

  function decrement() {
    count -= 1;
  }
</script>

<main>
  <h1>Counter</h1>
  <button on:click={decrement}>-</button>
  <span>{count}</span>
  <button on:click={increment}>+</button>
</main>
