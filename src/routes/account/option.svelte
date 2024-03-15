<script>

  /**
    * @type {string}
    */
   export var optionName;

</script>

<div class="accountOption">
  <div class="title unselectable">
    {optionName}
  </div>
</div>

<style>
  .accountOption {
    position: relative;
    width: auto;
    height: auto;
    background-color: var(--primary-color);
    box-shadow: 4px 4px 4px 0px rgba(0, 0, 0, 0.2);
    border-radius: 20px;
    justify-content: space-between;
    padding: 10px;
    padding-left: 20px;
    left: 0;
    transition: left 0.05s ease-in-out;
  }

  .accountOption:hover {
    cursor: pointer;
    left: 10px;
    transition: background-color 0.1s ease-in-out;
  }
  .accountOption:active {
    left: 10px;
    background-color: var(--accent-color);
    color: var(--primary-color);
  }

  .accountOption .title {
    color: var(--background-color);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 20px;
    font-weight: 400;
    transition: color 0.1s ease-in-out;
  }

  .accountOption:active .title {
    color: var(--primary-color);
  }

</style>
