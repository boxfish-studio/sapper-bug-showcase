<script>
  let divClientHeight,
    height = 20;
  $: console.log(divClientHeight);
</script>

<svelte:head>
  <title>About</title>
</svelte:head>

<input type="range" bind:value={height} />

<div
  style="background-color: blue; color:white; height: {height}px; width: 100px"
  bind:clientHeight={divClientHeight}>
  div content
</div>
