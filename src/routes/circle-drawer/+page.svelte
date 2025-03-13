<script>
  import { onMount } from 'svelte';

  let circles = [];
  let svgWidth = 500;
  let svgHeight = 500;

  onMount(() => {
    updateCanvasSize();
    window.addEventListener('resize', updateCanvasSize);
    return () => window.removeEventListener('resize', updateCanvasSize);
  });

  function updateCanvasSize() {
    svgWidth = Math.min(window.innerWidth - 40, 500);
    svgHeight = Math.min(window.innerHeight - 100, window.innerWidth - 40);
  }
  let radius = 10;

  function addCircle(event) {
    const { offsetX, offsetY } = event;
    circles = [...circles, { x: offsetX, y: offsetY, radius }];
  }
</script>

<main style="border: 1px solid black; padding: 10px;">
  <p>This task allows drawing and manipulating circles on a canvas.</p>
  <h1>Circle Drawer</h1>
  <div>
    <label for="radius">Radius:</label>
    <input type="range" id="radius" bind:value={radius} min="1" max="100" />
  </div>
  <svg
    on:click={addCircle}
    style="border: 1px solid black;"
    {svgWidth}
    {svgHeight}
  >
    {#each circles as { x, y, radius }}
      <circle cx={x} cy={y} r={radius} fill="blue" />
    {/each}
  </svg>
</main>
