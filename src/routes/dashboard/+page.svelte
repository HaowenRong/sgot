
<script>
  import NavBar from '../../components/navBar/navBar.svelte'
  import Board from '../../components/sessions/sessionBoard.svelte'

</script>

<style>
  .sessions-board {
    position: relative;
    display: flex;
    flex-direction: row;
    align-items: start;
    justify-content: center;
    gap: 20px;
    padding: 0px 20px 20px;
    flex-wrap: nowrap;
    margin: 100px 0px 0px;
  }

  @media (max-width: 950px) {
  .sessions-board {
    flex-direction: column;
  }
}
</style>



<div class="sessions-board">
  <Board boardName="Board name placeholder 1"/>
  <Board boardName="Board name placeholder 2"/>
</div>
