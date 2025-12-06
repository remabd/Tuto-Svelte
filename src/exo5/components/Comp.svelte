<script lang="ts">
  let num1 = $state(0);
  let num2 = $state(0);
  let sum = $derived(parseInt(num1.toString().split("")[0]) * 10 + (num2 % 10));
</script>

<h1>Somme: {sum}</h1>
<label for="champ-1">Un nombre</label>
<input
  id="champ-1"
  type="number"
  placeholder="un nombre"
  onchange={(e) => (num1 = parseInt(e.currentTarget.value))}
/>
<label for="champ-2">Un autre nombre</label>
<input
  id="champ-2"
  type="number"
  placeholder="un autre nombre"
  onchange={(e) => (num2 = parseInt(e.currentTarget.value))}
/>
