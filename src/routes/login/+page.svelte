<script>
  import LoginBoard from "./loginBoard.svelte";
  import LoginForm from "./loginForm.svelte";
</script>

<style>
  .container {
    height: 80vh;
    padding: 20px;
    margin-left:  20%;
    margin-right: 20%;
  }

  @media (max-width: 950px) {
    .container {
      margin-left:  0%;
      margin-right: 0%;
    }
  }
</style>

<div class="container">
  <LoginBoard>
    <LoginForm  />
  </LoginBoard>
</div>
