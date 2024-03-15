<script>
  import TextField    from "./textField.svelte";
  import SubmitButton from "./submitButton.svelte";

  /**
   * @type {string}
   */
  let username = '';

  /**
   * @type {string}
   */
  let password = '';

  /**
   * @type {string}
   */
  let usernameErrMsg = '';

  /**
   * @type {string}
   */
   let passwordErrMsg = '';

  function login() {
    console.log('do log in stuff')
  }
  function register() {
    console.log('do registration stuff')
  }
  
  function usernameCheck() {
    if (!(username.length <= 32)) {
      usernameErrMsg ='Username exceeds character limit. Current length:' + username.length;
    } else if (usernameErrMsg != '') {
      usernameErrMsg = '';
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


  @media (max-width: 950px) {
    .options-section {
      flex-direction: column;
      align-items: center;
    }
  }
</style>

<div class="credentials-section">
  <TextField type='text'     name="usernameField" id="username"
  bind:textValue={username} bind:errorMessage={usernameErrMsg} validation={usernameCheck} />
  <TextField type='password' name="passwordField" id="password"
  bind:textValue={password} bind:errorMessage={passwordErrMsg} validation={passwordCheck} />
</div>
<div class="options-section">
  <SubmitButton optionName='Login'    buttonFunc={login} />
  <SubmitButton optionName='Register' buttonFunc={register} />
</div>
