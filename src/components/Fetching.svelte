<script>
    import { onMount } from 'svelte';
    import axios from 'axios';

    export let url = 'https://swapi.co/api/people/';
    let dataarr = [];
    onMount(
        axios.get(url).then(res => {
            dataarr.push(res.data)
            console.log(dataarr)
        })
    );
</script>

<style>
    div {
        border: 1px solid greenyellow;
    }
</style>

<div>

</div>
