<script>
  import Option from "./option.svelte";

  const testArray = [1, 2, 3, 4, 5];
</script>

<div class="board">
  {#each testArray as num}
    <Option optionName="Option {num}"  />
  {/each}
</div>

<style>
  .board {
    position: relative;
    width: 100%;
    height: 100%;
    background-color: rgba(255, 255, 255, 1);
    box-sizing: border-box;
    padding: 40px;
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
</style>
