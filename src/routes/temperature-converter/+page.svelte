<script>
  let celsius = 0;
  let fahrenheit = 32;

  function convertToCelsius() {
    celsius = ((fahrenheit - 32) * 5) / 9;
  }

  function convertToFahrenheit() {
    fahrenheit = (celsius * 9) / 5 + 32;
  }
</script>

<main>
  <p>This task converts temperatures between Celsius and Fahrenheit.</p>
  <h1>Temperature Converter</h1>
  <div>
    <label>Celsius</label>
    <input type="number" bind:value={celsius} on:input={convertToFahrenheit} />
  </div>
  <div>
    <label>Fahrenheit</label>
    <input type="number" bind:value={fahrenheit} on:input={convertToCelsius} />
  </div>
</main>
