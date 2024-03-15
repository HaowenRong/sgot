<script>
  /**
    * @type {string}
    */
  export var optionName;

  /**
    * @type {(event: MouseEvent) => void}
    */
  export let buttonFunc;

</script>

<button class="accountOption" on:click={buttonFunc}>
  <div class="title unselectable">
    {optionName}
  </div>
</button>

<style>
  .accountOption {
    all: unset;
    position: relative;
    width: 100%;
    height: 25px;
    background-color: var(--primary-color);
    box-shadow: 4px 4px 4px 0px rgba(0, 0, 0, 0.2);
    border-radius: 15px;
    justify-content: space-between;
    padding: 10px;
    text-align: center;
    top: 0;
    transition: top 0.1s ease-in-out;
  }

  @media (max-width: 950px) {
    .accountOption {
      width: 70%;
    }
  }

  .accountOption:hover {
    cursor: pointer;
    top: -2px;
    transition: background-color 0.1s ease-in-out;
  }
  .accountOption:active {
    top: -2px;
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
