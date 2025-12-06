<script lang="ts">
  let rouge = $state(255);
  let bleu = $state(255);
  let vert = $state(255);
  $inspect(rouge);
</script>

<label for="chp_r">Niveau de rouge&thinsp;: </label><input
  onchange={(e) => (rouge = parseInt(e.currentTarget.value))}
  type="range"
  min="0"
  max="255"
  id="chp_r"
/>
<label for="chp_v">Niveau de vert&thinsp;: </label><input
  onchange={(e) => (vert = parseInt(e.currentTarget.value))}
  type="range"
  min="0"
  max="255"
  id="chp_v"
/>
<label for="chp_b">Niveau de bleu&thinsp;: </label><input
  onchange={(e) => (bleu = parseInt(e.currentTarget.value))}
  type="range"
  min="0"
  max="255"
  id="chp_b"
/>

<div id="temoin" style="background-color: rgb({rouge}, {vert}, {bleu});">
  <p>J'aime le rgb</p>
</div>

<style>
</style>
