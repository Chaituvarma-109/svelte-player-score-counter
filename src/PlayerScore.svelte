<script>
    export let playerName;
    export let playerScore = 0;

    function decreaseScore() {
        playerScore--
        if (playerScore < 0) {
            playerScore = 0
        }
    }
</script>

<div>
    <h3 class="center">{playerName}</h3>
    <button on:click={() => playerScore++}>up</button>
    <h1 class="center">{playerScore}</h1>
    <button on:click={decreaseScore}>down</button>
</div>

<style>
    .center{
        text-align: center;
    }
</style>
