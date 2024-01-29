
<script>
  import NavBar from '../components/navBar/navBar.svelte'
  import SessionsBoard from '../components/sessions/sessionBoard.svelte'
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
</style>

<NavBar />

<div class="sessions-board">
  <SessionsBoard />
  <SessionsBoard />
</div>
