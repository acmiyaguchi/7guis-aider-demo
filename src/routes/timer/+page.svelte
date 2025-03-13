<script>
  let time = 0;
  let interval;

  function start() {
    if (!interval) {
      interval = setInterval(() => {
        time += 1;
      }, 1000);
    }
  }

  function stop() {
    clearInterval(interval);
    interval = null;
  }

  function reset() {
    time = 0;
    stop();
  }
</script>

<main style="border: 1px solid black; padding: 10px;">
  <p>This task is a countdown timer with start, stop, and reset functionality.</p>
  <h1>Timer</h1>
  <div>{time} seconds</div>
  <button on:click={start}>Start</button>
  <button on:click={stop}>Stop</button>
  <button on:click={reset}>Reset</button>
</main>
