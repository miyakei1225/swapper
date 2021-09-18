<script lang="ts">
  import Button, { Label } from "@smui/button";

  let count: number = 0;
  const increment = () => {
    count += 1;
  };
</script>

<div>
  <Button color="secondary" on:click={increment}>
    <Label>Default</Label>
  </Button>
  <Button color="secondary" on:click={increment} disabled>
    <Label>Disabled</Label>
  </Button>
  <Button color="secondary" on:click={increment} ripple={false}>
    <Label>No Ripple</Label>
  </Button>
  <Button color="secondary" on:click={increment} class="myClass">
    <Label>With a Class</Label>
  </Button>
</div>
<pre>Click: {count}</pre>

<style>
</style>
