<script>
    //a very basic clicker used for our svelte kit demo.
    //the logic that defines clicks per click and handles the actual click
    let clicksPerClick = 1;
    let clicks = 0;
    function buttonClick() {
        clicks += clicksPerClick;
    }
</script>

<h1>Click:</h1>

<button on:click={buttonClick}>Click Me</button>
<p>Balance: {clicks}</p>

<h1>Upgrades:</h1>
