<script>

  /**
    * @type {string}
    */
   export var optionName;

</script>

<div class="accountOption">
  <div class="title">
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
    border-radius: 18px;
    justify-content: space-between;
    padding: 10px;
    padding-left: 20px;
  }

  .accountOption:hover {
    cursor: pointer;
  }

  .accountOption .title {
    color: var(--background-color);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 20px;
    font-weight: 400;
  }

</style>
