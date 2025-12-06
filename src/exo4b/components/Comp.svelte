<script lang="ts">
  let tab: number[] = $state([]);
  let count = $state(0);
  let result = $derived(tab.reduce((acc, curr) => acc + curr, 0));

  function start() {
    for (let i = 0; i < 1000; i++) {
      tab.push(Math.pow(-1, i) / (2 * i + 1));
    }
  }

  $inspect(result);
</script>

<p>{4 * result}</p>
<button onclick={start}>Bouton!</button>
