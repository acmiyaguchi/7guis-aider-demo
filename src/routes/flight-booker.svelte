<script>
  let flightType = 'one-way';
  let startDate = '';
  let returnDate = '';

  function bookFlight() {
    alert(`Flight booked: ${flightType} from ${startDate} to ${returnDate}`);
  }
</script>

<main>
  <h1>Flight Booker</h1>
  <select bind:value={flightType}>
    <option value="one-way">One-way</option>
    <option value="return">Return</option>
  </select>
  <input type="date" bind:value={startDate} />
  {#if flightType === 'return'}
    <input type="date" bind:value={returnDate} />
  {/if}
  <button on:click={bookFlight}>Book</button>
</main>
