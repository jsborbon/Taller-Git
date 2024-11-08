<script lang="ts">
  let count: number = $state(0)

  const increment = () => {
    if(count === 20) {
      alert('You have reached the maximum limit')
      }else {
      count += 1
    }
  }
  const decrement = () => {
    if(count === 0) {
      alert('You have reached the minimum limit')
      }else {
    count -= 1
  }
    }

</script>

<input type="text" bind:value={count} readonly />
<button onclick={increment}>
  Start
</button>

<button onclick={decrement}>
  Dicrease -
</button>
