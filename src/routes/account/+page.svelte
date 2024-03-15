<script>
  import AccountBoard from "./accountBoard.svelte";
  import OptionsBoard from "./optionsBoard.svelte";
</script>

<div class="container">
  <div class="accountSection">
    <AccountBoard accountName="Placeholder Name" accountCreation="2025/12/25"  />
  </div>
  <div class="optionsSection">
    <OptionsBoard  />
  </div>
</div>

<style>
  .container {
    height: 80vh;
    padding: 20px;
    display: flex;
  }
  
  .accountSection {
    width: 40%;
    height: 100%;
  }

  .optionsSection {
    width: 60%;
    height: 100%;
  }

  @media (max-width: 950px) {
    .container {
      flex-direction: column;
    }

    .accountSection {
      width: 100%;
      height: 100%;
    }

    .optionsSection {
      width: 100%;
      height: 100%;
    }
  }

</style>
