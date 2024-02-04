<script>
	/**
     * @type {string}
     */
	 export var currPage;
</script>

<div class="navBarContainer">
  <div class="left">
    <div class="title">
      SGOT
    </div>
  </div>
  <div class="middle">
    <div class="content">
      <div class="icon">

      </div>
      <div class="title">
        {currPage}
      </div>
    </div>
  </div>
  <div class="right">
    <div class="accounts-pill">
      <div class="account-name">
        Accounts
      </div>
      <div class="account-picture">

      </div>
    </div>
  </div>
</div>

<style>
  @import '/styles/variables.css';
	.navBarContainer {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: var(--nav-height);
    background-color: rgba(255, 255, 255, 1);
    box-shadow: 0px 10px 5px 0px rgba(0, 0, 0, 0.1);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    gap: 0px;
    padding: 0px 0px;
    flex-wrap: nowrap;
  }

  .navBarContainer .left {
    position: relative;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: start;
    gap: 0px;
    padding: 50px;
    flex-wrap: nowrap;
    align-self: center;
  }

  .navBarContainer .left .title {
    width: auto;
    color: rgba(69, 71, 75, 1);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 28px;
    font-weight: 400;
  }
  .navBarContainer .left .title:hover {
    cursor: pointer;
  }

  .navBarContainer .middle {
    position: relative;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    gap: 0px;
    padding: 0px;
    flex-wrap: nowrap;
  }

  .navBarContainer .middle .content {
    width: auto;
    height: auto;
    background-color: rgba(255, 255, 255, 0);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    gap: 10px;
    padding: 10px;
    flex-wrap: nowrap;
    align-self: center;
  }

  .navBarContainer .middle .content .icon {
    position: relative;
    background: url(https://api.iconify.design/carbon:user-avatar-filled.svg) center/cover no-repeat;
    order: -1;
    width: 32px;
    height: 32px;
  }

  .navBarContainer .middle .content .title {
    width: auto;
    height: 100%;
    color: rgba(69, 71, 75, 1);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 32px;
    font-weight: 400;
  }

  .navBarContainer .right {
    position: relative;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: end;
    gap: 0px;
    padding: 50px;
    flex-wrap: nowrap;
  }

  .accounts-pill {
    position: relative;
    width: auto;
    height: 20px;
    border-radius: 40px;
    background-color: rgba(240, 240, 240, 1);
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    justify-content: start;
    padding: 10px 5px 10px 5px;
    flex-wrap: nowrap;
  }

  .accounts-pill .account-name {
    width: auto;
    height: auto;
    margin: 0px 10px;
    color: rgba(69, 71, 75, 1);
    font-family: 'Noto Emoji';
    font-style: normal;
    font-size: 28px;
    font-weight: 400;
  }

  .accounts-pill .account-picture {
    order: -1;
    background: url(https://api.iconify.design/carbon:user-avatar-filled.svg) center/cover no-repeat;
    width:  35px;
    height: 35px;
  }

</style>
