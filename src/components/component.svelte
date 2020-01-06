<script>
let value = 42;
export let batosha = 24;
</script>

<style>
div {
    border: 1px solid red;
}
</style>

<div>
<h3>Hello from here</h3>
<slot />
<h3>{batosha}</h3>
</div>
