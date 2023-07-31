<script>
  import PlayerScore from "./PlayerScore.svelte";

  let player1Score = 0;
  let player2Score = 0;

  function reset() {
    player1Score = 0;
    player2Score = 0;
  }
</script>

<main>
  <PlayerScore bind:playerScore={player1Score} playerName='player1' />
  <PlayerScore bind:playerScore={player2Score} playerName='player2' />
  <button on:click={reset} class="contrat outline">Reset</button>
</main>
