<script>
  import Session from "./session.svelte";

	/**
     * @type {string}
     */
	 export var boardName;
  const testArray = [1, 2, 3, 4, 5];
</script>

<div class=boardContainer>
  <div class="pill">
    <div class="icon">

    </div>
    <div class="title unselectable">
      {boardName}
    </div>
  </div>
  <div class=board>
    <div class="inner">

      {#each testArray as num}
        <Session sessionName="Placeholder name {num}"
                 lastUsed   ="2025/12/25"/>
      {/each}

      <!--
      <div class="body">
        <div class="button">
          View session
        </div>
        <div class="button">
          Manage session
        </div>
      </div>
      -->

    </div>
  </div>
</div>

<style>
  .boardContainer {
    width: 100%;
    height: auto;
    position: relative;
    margin: auto;
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    gap: 0px;
    padding: 20px;
    flex-wrap: nowrap;
  }

  .board {
    position: relative;
    width: 100%;
    height: auto;
    border-radius: 20px;
    background-color: var(--background-color);
    border: 2px solid var(--primary-color);
    box-sizing: border-box;
    padding: 20px;
    margin-top: 18px;
  }

  .board .inner {
    border-radius: 20px;
    position: relative;
    width: 100%;
    height: auto;
    margin: 18px 0px 0px 0px;
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    gap: 20px;
    flex-wrap: nowrap;
    z-index: 0;
  }

  .pill {
    position: absolute;
    width: auto;
    height: auto;
    border-radius: 50px;
    background-color: var(--background-color);
    display: flex;
    gap: 5px;
    flex-direction: row;
    align-items: center;
    justify-content: start;
    padding: 5px 5px;
    margin: 0px 0px 0px 30px;
    z-index: 1;
  }

  .pill .icon {
    position: relative;
    background: url(https://api.iconify.design/carbon:user-avatar-filled.svg) center/cover no-repeat;
    order: -1;
    width: 30px;
    height: 30px;
  }

  .pill .title {
    height: 100%;
    color: var(--primary-color);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 22px;
    font-weight: 400;
    line-height: 1.0;
    letter-spacing: 0px;
    text-decoration: none;
    text-transform: none;
    padding-right: 5px;
  }
</style>
