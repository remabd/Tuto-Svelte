<script lang="ts">
  const nb = Math.floor(Math.random() * 10 + 1);
  let nbTentatives = $state(0);
  let ecart: number | undefined = $state(undefined);
  function test() {
    const value = document.getElementById("nb")?.value;
    console.log(value);
    ecart = Math.abs(parseInt(value) - nb);
    nbTentatives++;
  }
</script>

<label for="nb">Saisissez un nombre compris entre 1 et 10</label><input
  type="number"
  min="1"
  max="10"
  id="nb"
  value="5"
/>
<button onclick={test}>Testez-le!</button>
<p>Au-dessus!</p>
<p>En dessous!</p>
<p>Gagné en {nbTentatives} coups</p>
