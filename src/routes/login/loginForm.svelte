<script>
  import TextField from "./textField.svelte";

  /**
   * @type {string}
   */
  let userName = '';

  /**
   * @type {string}
   */
  let password = '';

  function login() {
    console.log("login");
  }
  function register() {
    console.log("register");
  }
  
  function usernameCheck() {
    if (!(userName.length <= 32)) {
      userName = userName;
    }
  }
  function passwordCheck() {
    if (!(password.length >= 8 &&
          password.length <= 100)) {
    }
  }
</script>

<style>
  /* sections */
  .credentials-section {
    display: flex;
    flex-direction: column;
    width: 100%;
    height: calc(100% - 50px);
    gap: 20px;
  }

  .options-section {
    display: flex;
    width: 100%;
    height: 30%;
    gap: 20px;
  }

  /* buttons */
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


  @media (max-width: 950px) {
    .options-section {
      flex-direction: column;
      align-items: center;
    }

    .accountOption {
      width: 70%;
    }
  }
</style>

<div class="credentials-section">
  <div>{userName}</div>
  <div>{password}</div>
  <TextField type='text'     name="userNameField" id="userName"
  bind:textValue={userName} validation={usernameCheck} />
  <TextField type='password' name="passwordField" id="password"
  bind:textValue={password} validation={passwordCheck} />
</div>
<div class="options-section">
  <button class="accountOption" on:click={login}>
    <div class="title unselectable">
      Login
    </div>
  </button>
  <button class="accountOption" on:click={register}>
    <div class="title unselectable">
      Register
    </div>
  </button>
</div>
