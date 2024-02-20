<script>
  import OptionButton from "./optionButton.svelte";

  const options = ["Allocate Players", "View Players", "Add Players", "View Scores", "Session Settings"];

  function allocatePlayers() {
    console.log("allocatePlayers");
  }
  function viewPlayers() {
    console.log("viewPlayers");
  }
  function addPlayers() {
    console.log("addPlayers");
  }
  function viewScores() {
    console.log("viewScores");
  }
  function sesstionSettings() {
    console.log("sesstionSettings");
  }
</script>

<div class="board">
  <OptionButton optionName="Allocate Players" buttonFunc={allocatePlayers} />
  <OptionButton optionName="View Players"     buttonFunc={viewPlayers} />
  <OptionButton optionName="Add Players"      buttonFunc={addPlayers} />
  <OptionButton optionName="View Scores"      buttonFunc={viewScores} />
  <OptionButton optionName="Session Settings" buttonFunc={sesstionSettings} />
</div>

<style>
  .board {
    position: relative;
    border-radius: 20px;
    background-color: var(--background-color);
    border: 2px solid var(--primary-color);
    box-sizing: border-box;
    padding: 10px;
    display: flex;
    gap: 10px;
    overflow: scroll;
  }
</style>
