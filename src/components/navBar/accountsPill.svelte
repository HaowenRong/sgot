<script>
  /**
     * @type {string}
     */
   export var accountName;
</script>

<a href='./account' class="accounts-pill">
  <div class="account-name">
    {accountName}
  </div>
  <svg class="account-picture" xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 32 32">
    <path fill="none" d="M8.007 24.93A4.996 4.996 0 0 1 13 20h6a4.996 4.996 0 0 1 4.993 4.93a11.94 11.94 0 0 1-15.986 0M20.5 12.5A4.5 4.5 0 1 1 16 8a4.5 4.5 0 0 1 4.5 4.5"/>
    <path fill="currentColor" d="M26.749 24.93A13.99 13.99 0 1 0 2 16a13.899 13.899 0 0 0 3.251 8.93l-.02.017c.07.084.15.156.222.239c.09.103.187.2.28.3c.28.304.568.596.87.87c.092.084.187.162.28.242c.32.276.649.538.99.782c.044.03.084.069.128.1v-.012a13.901 13.901 0 0 0 16 0v.012c.044-.031.083-.07.128-.1c.34-.245.67-.506.99-.782c.093-.08.188-.159.28-.242c.302-.275.59-.566.87-.87c.093-.1.189-.197.28-.3c.071-.083.152-.155.222-.24ZM16 8a4.5 4.5 0 1 1-4.5 4.5A4.5 4.5 0 0 1 16 8M8.007 24.93A4.996 4.996 0 0 1 13 20h6a4.996 4.996 0 0 1 4.993 4.93a11.94 11.94 0 0 1-15.986 0"/>
  </svg>
</a>

<style>
  .accounts-pill {
    all: unset;
    position: relative;
    width: auto;
    height: 20px;
    border-radius: 40px;
    background-color: var(--accent-color);
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    justify-content: start;
    padding: 10px 5px 10px 5px;
    flex-wrap: nowrap;
  }

  .accounts-pill:hover {
    cursor: pointer;
  }

  .accounts-pill:active {
    top: -2px;
  }

  .accounts-pill .account-name {
    width: auto;
    height: auto;
    margin: 0px 10px;
    color: var(--primary-color);
    font-family: 'Noto Emoji';
    font-style: normal;
    font-size: 20px;
    font-weight: 400;
  }

  .accounts-pill .account-picture {
    order: -1;
    background: url(https://api.iconify.design/carbon:user-avatar-filled.svg) center/cover no-repeat;
    width:  35px;
    height: 35px;
    color: var(--primary-color);
  }
</style>
