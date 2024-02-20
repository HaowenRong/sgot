<script>
  import SessionInfo from "./sessionInfo.svelte";
  import SessionOptions from "./sessionOptions.svelte";
  import ActiveMatches from "./activeMatches.svelte";
</script>

<div class="mainBody">
  <div class="session-info">
    <SessionInfo  />
  </div>
  <div class="session-options">
    <SessionOptions  />
  </div>

  <div class="active-sessions">
    <ActiveMatches  />
  </div>
</div>

<style>
  .mainBody {
    left: 0px;
    margin-top: calc(var(--nav-height) + 40px);
    height: 80vh;
    padding: 20px;
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  
  .session-info {
    height: auto;
    width: 100%;
  }

  .session-options {
    height: auto;
    width: 100%;
  }

  .active-sessions {
    height: auto;
    width: 100%;
  }

</style>
