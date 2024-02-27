<script>
  import AccountsPill from "./accountsPill.svelte";
  
	/**
     * @type {string}
     */
	 export var currPage;
</script>

<div class="navBarContainer unselectable">
  <div class="left">
    <a href='./dashboard' class="title">
      SGOT
    </a>
  </div>
  <div class="middle">
    <div class="content">
      <svg class="icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32">
        <path fill="currentColor" d="M8 30H4a2 2 0 0 1-2-2v-4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v4a2 2 0 0 1-2 2m-4-6v4h4v-4zm14 6h-4a2 2 0 0 1-2-2v-4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v4a2 2 0 0 1-2 2m-4-6v4h4v-4zm14 6h-4a2 2 0 0 1-2-2v-4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v4a2 2 0 0 1-2 2m-4-6v4h4v-4zM8 20H4a2 2 0 0 1-2-2v-4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v4a2 2 0 0 1-2 2m-4-6v4h4v-4zm14 6h-4a2 2 0 0 1-2-2v-4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v4a2 2 0 0 1-2 2m-4-6v4h4v-4zm14 6h-4a2 2 0 0 1-2-2v-4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v4a2 2 0 0 1-2 2m-4-6v4h4v-4zM8 10H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v4a2 2 0 0 1-2 2M4 4v4h4V4zm14 6h-4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v4a2 2 0 0 1-2 2m-4-6v4h4V4zm14 6h-4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v4a2 2 0 0 1-2 2m-4-6v4h4V4z"/>
      </svg>
      <div class="title">
        {currPage}
      </div>
    </div>
  </div>
  <div class="right">
    <AccountsPill accountName="Account" />
  </div>
</div>

<style>
  @import '/styles/variables.css';
  @import '/styles/common.css';
	.navBarContainer {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: var(--nav-height);
    background-color: var(--background-color);
    box-shadow: 0px 10px 5px 0px rgba(0, 0, 0, 0.1);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    gap: 0px;
    padding: 0px 0px;
    flex-wrap: nowrap;
    z-index: 9999;
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
    all: unset;
    width: auto;
    color: var(--primary-color);
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
    order: -1;
    width: 28px;
    height: 28px;
    color: var(--primary-color);
  }

  .navBarContainer .middle .content .title {
    width: auto;
    height: 100%;
    color: var(--primary-color);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 24px;
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

</style>
