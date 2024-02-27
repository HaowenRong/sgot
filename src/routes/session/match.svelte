<script>

  /**
     * @type {String}
     */
   export var matchTitle;
  
  /**
     * @type {any}
     */
   export var matchScoreLeft;

  /**
     * @type {any}
     */
   export var matchScoreRight;

  /**
     * @type {any}
     */
   export var startTime;
  
  /**
     * @type {string | any[]}
     */
   export var playersLeft;
  /**
     * @type {any[]}
     */
   export var playersRight;

  /**
     * @type {number}
     */
  var type;

  if (playersLeft.length == 1) {
    type = 1;
  } else if (playersLeft.length == 2) {
    type = 2;
  } else {
    type = 0;
  }

</script>

<div class="match-board">
  <div class="heading">
    <div class="title">
      {matchTitle}
    </div>

    <div class="score">
      <div class="left">
        {matchScoreLeft}
      </div>
      <div class="seperator">
        -
      </div>
      <div class="right">
        {matchScoreRight}
      </div>
    </div>

    <div class="start-time">
      {startTime}
    </div>
  </div>
  <div class="content">
    <div class="court-side">
      <div class="left">

        <div class="player" draggable="true">
          <div class="name">
            {playersLeft[0]}
          </div>
        </div>

        {#if playersLeft.length == 2}
          <div class="player" draggable="true">
            <div class="name">
              {playersLeft[1]}
            </div>
          </div>
        {/if}

      </div>
    </div>
    <div class="court-side">
      <div class="right">

        <div class="player" draggable="true">
          <div class="name">
            {playersRight[0]}
          </div>
        </div>

        {#if playersRight.length == 2}
          <div class="player" draggable="true">
            <div class="name">
              {playersRight[1]}
            </div>
          </div>
        {/if}

      </div>

    </div>
  </div>
</div>

<style>
  .match-board {
    width: auto;
    max-width: 1000px;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 4px 4px 4px 0px rgba(0, 0, 0, 0.2);
    display: flex;
    flex-direction: column;
    justify-content: start;
    flex-wrap: nowrap;
    align-self: start;
    flex-grow: 1;
  }

  /* Heading */
  .match-board .heading {
    background-color: var(--primary-color);
    padding: 20px 10px 0px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    gap: 20px;
    padding: 30px 20px 0px;
    flex-wrap: nowrap;
    color: var(--background-color);
  }

  .match-board .heading .title {
    width: 100%;
    font-size: x-large;
    text-align: left;
  }

  .match-board .heading .score {
    width: 100%;
    font-size: x-large;
    display: flex;
    justify-content: space-between;
    gap: 10px;
  }

  .match-board .heading .score .left {
    width: 100%;
    align-self: right;
    text-align: right;
  }
  .match-board .heading .score .seperator {
    width: auto;
  }
  .match-board .heading .score .right {
    width: 100%;
    align-self: left;
    text-align: left;
  }

  .match-board .heading .start-time {
    width: 100%;
    font-size: large;
    text-align: right;
  }

  /* Content */
  .match-board .content {
    background-color: var(--background-color);
    display: flex;
    flex-direction: row;
    align-items: start;
    justify-content: start;
    gap: 0px;
    padding: 0px;
    flex-wrap: nowrap;
  }

  .court-side {
    position: relative;
    width: 100%;
    height: auto;
    background-color: var(--background-color);
    display: flex;
    flex-direction: column;
    gap: 0px;
    padding: 0px;
    flex-wrap: nowrap;
  }

  .court-side .left {
    display: flex;
    flex-direction: column;
    align-items: start;
    border-right: 5px solid var(--primary-color);
  }
  .court-side .right {
    display: flex;
    flex-direction: column;
    align-items: end;
    border-left: 5px solid var(--primary-color);
  }

  .player {
    position: relative;
    min-width: 250px;
    max-width: 500px;
    height: auto;
    background-color: var(--background-color);
    display: flex;
    flex-direction: column;
    align-items: inherit;
    justify-content: start;
    gap: 0px;
    flex-wrap: nowrap;
  }
  .player .name {
    color: var(--primary-color);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 20px;
    font-weight: 400;
    padding: 10px;
  }
</style>
