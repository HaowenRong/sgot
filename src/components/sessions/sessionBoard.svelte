<script>
	// logic goes here
</script>

<div class=boardContainer>
  <div class="pill">
    <div class="icon">

    </div>
    <div class="title">
      Sessions
    </div>
  </div>
  <div class=board>
    <div class="inner">

      <div class="sessionBoard">
        <div class="heading">
          <div class="title">
            Session Name
          </div>
          <div class="lastUsed">
            Last used: 2025/12/25
          </div>
          <svg class="settingsIcon" />
        </div>
        <div class="body">
          <div class="button">
            View session
          </div>
          <div class="button">
            Manage session
          </div>
        </div>
      </div>

      <div class="sessionBoard">
        <div class="heading">
          <div class="title">
            Session Name
          </div>
          <div class="lastUsed">
            Last used: 2025/12/25
          </div>
          <svg class="settingsIcon" />
        </div>
      </div>

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
    background-color: rgba(255, 255, 255, 1);
    border: 2px solid rgba(69, 71, 75, 1);
    box-sizing: border-box;
    padding: 20px;
    margin-top: 18px;
  }

  .board .header {
    position: absolute;
    top: 0px;
    left: 0px;
    width: 100%;
    height: 38px;
    background-color: rgba(255, 255, 255, 1);
    z-index: 1;
    overflow: hidden;
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
    background-color: rgba(255, 255, 255, 1);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: start;
    gap: 5px;
    padding: 5px 5px;
    flex-wrap: nowrap;
    margin: 0px 0px 0px 40px;
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
    color: rgba(69, 71, 75, 1);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 20px;
    font-weight: 400;
    line-height: 1.0;
    letter-spacing: 0px;
    text-decoration: none;
    text-transform: none;
    padding-right: 5px;
  }

  /* sessions board */
  .sessionBoard {
    position: relative;
    width: 100%;
    height: auto;
    border-radius: 15px;
    background-color: rgba(255, 255, 255, 1);
    box-shadow: 4px 4px 4px 0px rgba(0, 0, 0, 0.2);
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    flex-wrap: nowrap;
    align-self: start;
    overflow: hidden;
  }

  .sessionBoard .heading {
    position: relative;
    width: 100%;
    height: auto;
    background-color: rgba(69, 71, 75, 1);
    display: flex;
    flex-direction: column;
    align-items: baseline;
    justify-content: space-between;
    gap: 0px;
    padding: 0px 0px 0px;
    flex-wrap: nowrap;
  }

  .sessionBoard .heading .title {
    color: rgba(255, 255, 255, 1);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 22px;
    font-weight: 400;
    
    letter-spacing: 0px;
    margin-top: 10px;
    margin-left: 10px;
  }

  .sessionBoard .heading .title:hover {
    cursor: pointer;
  }

  .sessionBoard .heading .lastUsed {
    color: rgba(255, 255, 255, 1);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 16px;
    font-weight: 400;
    letter-spacing: 0px;
    margin-right: 10px;
    margin-bottom: 10px;
  }

  .sessionBoard .heading .settingsIcon {
    position: fixed;
    align-self: self-end;
    background: url(https://api.iconify.design/carbon:settings.svg) center/cover no-repeat;
    order: 9999;
    width: 30px;
    height: 30px;
    margin: 10px;
  }

  .sessionBoard .heading .settingsIcon:hover {
    cursor: pointer;
  }

  .sessionBoard .body {
    position: relative;
    width: 100%;
    height: auto;
    background-color: rgba(255, 255, 255, 1);
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
