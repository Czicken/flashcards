<script lang="ts">
    import cards from "./cards.json";

    let counter = 0;
    function onClick() {}
</script>

<div>
    <h1>{cards[0].answer}</h1>
    {counter}
    <button on:click={onClick}>Click me</button>
</div>

<style lang="scss">
    h1 {
        color: red;
    }
</style>
