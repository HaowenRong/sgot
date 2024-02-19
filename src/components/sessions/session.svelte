<script>

   /**
     * @type {string}
     */
    export var sessionName;

   /**
     * @type {string}
     */
    export var lastUsed;
</script>


<div class="sessionBoard">
  <div class="heading">
    <div class="title">
      {sessionName}
    </div>
    <div class="lastUsed">
      Last used: {lastUsed}
    </div>
  </div>
  <svg class="settingsIcon" />
</div>

<style>
    .sessionBoard {
    position: relative;
    width: 100%;
    height: auto;
    border-radius: 18px;
    background-color: var(--background-color);
    box-shadow: 4px 4px 4px 0px rgba(0, 0, 0, 0.2);
    display: flex;
    flex-direction: row;
    align-items: start;
    justify-content: start;
    flex-wrap: nowrap;
    align-self: start;
    overflow: hidden;
  }

  .sessionBoard .heading {
    position: relative;
    width: calc(100% - 60px);
    height: auto;
    background-color: var(--primary-color);
    box-shadow: 4px 0px 4px 0px rgba(0, 0, 0, 0.2);
    border-radius: 18px;
    display: flex;
    flex-direction: column;
    align-items: baseline;
    justify-content: space-between;
    gap: 0px;
    padding: 10px;
    padding-left: 20px;
    flex-wrap: nowrap;
  }

  .sessionBoard .heading .title {
    color: var(--background-color);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 20px;
    font-weight: 400;
    
    width: 100%;
  }

  .sessionBoard .heading .title:hover {
    cursor: pointer;
  }

  .sessionBoard .heading .lastUsed {
    color: var(--background-color);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 16px;
    font-weight: 400;
    letter-spacing: 0px;
  }

  .sessionBoard .settingsIcon {
    position: relative;
    align-self: center;
    background: url(https://api.iconify.design/carbon:settings.svg) center/cover no-repeat;
    order: 9999;
    width: 30px;
    height: 30px;
    margin: 10px;
  }

  .sessionBoard .settingsIcon:hover {
    cursor: pointer;
  }

  .sessionBoard .body {
    position: relative;
    width: 100%;
    height: auto;
    background-color: var(--background-color);
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    gap: 10px;
    flex-wrap: nowrap;
  }

  .sessionBoard .body .button {
    position: relative;
    width: 100%;
    height: auto;
    border-radius: 50px;
    background-color: rgba(240, 240, 240, 1);
  }

  .sessionBoard .body .button:hover {
    cursor: pointer;
  }
</style>