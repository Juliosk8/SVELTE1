<script>
  import ParImpar from "./lib/parImpar.svelte";
  let valor = 0;

  const listentInput = (event) => (valor = event.target.value);
</script>

<main>
  <ParImpar numero={valor} />

  <input value={valor} on:input={listentInput} />
</main>
