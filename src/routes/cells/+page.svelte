<script>
  let cells = Array(10).fill('').map(() => Array(10).fill(''));

  function updateCell(row, col, event) {
    cells[row][col] = event.target.value;
  }
</script>

<main style="border: 1px solid black; padding: 10px;">
  <p>This task is a simple spreadsheet-like application.</p>
  <h1>Cells</h1>
  <table>
    {#each cells as row, rowIndex}
      <tr>
        {#each row as cell, colIndex}
          <td>
            <input type="text" bind:value={cells[rowIndex][colIndex]} on:input={(e) => updateCell(rowIndex, colIndex, e)} />
          </td>
        {/each}
      </tr>
    {/each}
  </table>
</main>
