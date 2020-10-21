<script>

export let time = 0;

const pause = () => {
  clearInterval(timer);
}

let timer = setInterval(() => {
  time++;
}, 1000)

</script>

<div>
  <h1>
  {time}
  </h1>

  <button on:click={pause}>
  Pause</button>
</div>


<style>
h1 {
  background: orange;
}
</style>