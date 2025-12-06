<script>
  let count = $state(0);

  function increment() {
    count++;
  }

  function decrement() {
    count--;
  }
</script>

<h1>{count}</h1>
<button onclick={increment}> Increment </button>
<button onclick={decrement}> Decrement </button>
