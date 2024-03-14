<script>
</script>

<div class=boardContainer>
  <div class="pill">
    <div class="icon">

    </div>
    <div class="title unselectable">
      Login
    </div>
  </div>
  <div class=board>
    <slot> </slot>
  </div>
</div>

<style>
  .boardContainer {
    width: 100%;
    height: auto;
    position: relative;
    display: flex;
    align-items: start;
    justify-content: start;
    gap: 0px;
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

    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
    gap: 20px;
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
