<script>
  let count = 0;

  function increment() {
    count += 1;
  }

  function decrement() {
    count -= 1;
  }
</script>

<main style="border: 1px solid black; padding: 10px;">
  <p>This task is a simple counter that can be incremented and decremented.</p>
  <h1>Counter</h1>
  <button on:click={decrement}>-</button>
  <span>{count}</span>
  <button on:click={increment}>+</button>
</main>
