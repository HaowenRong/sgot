<script>
  /**
     * @type {String}
     */
   export let type;
  /**
     * @type {String}
     */
   export let name;
  /**
     * @type {String}
     */
   export let id;
  /**
     * @type {string}
     */
   export let textValue;
  
  /**
     * @type {any}
     */
   export let validation;
</script>

<style>
  .textField {
    all: unset;
    position: relative;
    width: 95%;
    height: 25px;
    background-color: var(--accent-color);
    box-shadow: 4px 4px 4px 0px rgba(0, 0, 0, 0.2);
    border-radius: 15px;
    justify-content: space-between;
    padding: 10px;
    padding-left: 20px;
    top: 0;
    transition: top 0.1s ease-in-out;
  }
</style>

<div>
  {#if type === 'password'}
    <input type='password' name={name} id={id}
           class="textField"
           bind:value={textValue} on:input={validation}>
  {:else}
    <input type='text' name={name} id={id}
           class="textField"
           bind:value={textValue} on:input={validation}>
  {/if}
</div>
