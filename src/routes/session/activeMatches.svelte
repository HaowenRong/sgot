<script>
  import Match from "./match.svelte";
</script>

<div class=boardContainer>
  <div class="pill">
    <div class="icon">

    </div>
    <div class="title unselectable">
      Active Matches
    </div>
  </div>
  <div class=board>
    <Match matchTitle="Title"
           matchScoreLeft="15"
           matchScoreRight="15"
           startTime="Today at 15:00"
           playersLeft={["P1", "P2"]}
           playersRight={["P3", "P4"]}  />

    <Match matchTitle="Title"
           matchScoreLeft="15"
           matchScoreRight="15"
           startTime="Today at 15:00"
           playersLeft={["P1", "P2"]}
           playersRight={["P3", "P4"]}  />
    
    <Match matchTitle="Title"
           matchScoreLeft="15"
           matchScoreRight="15"
           startTime="Today at 15:00"
           playersLeft={["P1", "P2"]}
           playersRight={["P3", "P4"]}  />
    <Match matchTitle="Title"
           matchScoreLeft="15"
           matchScoreRight="15"
           startTime="Today at 15:00"
           playersLeft={["P1", "P2"]}
           playersRight={["P3", "P4"]}  />

    <Match matchTitle="Title"
           matchScoreLeft="15"
           matchScoreRight="15"
           startTime="Today at 15:00"
           playersLeft={["P1", "P2"]}
           playersRight={["P3", "P4"]}  />
    
    <Match matchTitle="Title"
           matchScoreLeft="15"
           matchScoreRight="15"
           startTime="Today at 15:00"
           playersLeft={["P1", "P2"]}
           playersRight={["P3", "P4"]}  />

    <Match matchTitle="Title"
           matchScoreLeft="15"
           matchScoreRight="15"
           startTime="Today at 15:00"
           playersLeft={["P1", "P2"]}
           playersRight={["P3", "P4"]}  />

    <Match matchTitle="Title"
           matchScoreLeft="15"
           matchScoreRight="15"
           startTime="Today at 15:00"
           playersLeft={["P1", "P2"]}
           playersRight={["P3", "P4"]}  />
    
    <Match matchTitle="Title"
           matchScoreLeft="15"
           matchScoreRight="15"
           startTime="Today at 15:00"
           playersLeft={["P1", "P2"]}
           playersRight={["P3", "P4"]}  />
  </div>
</div>

<style>
  .boardContainer {
    margin-top: -10px;
    width: 100%;
    height: 70vh;
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    gap: 0px;
    flex-wrap: nowrap;
  }

  .board {
    position: relative;
    width: 100%;
    height: 100%;
    border-radius: 20px;
    background-color: var(--background-color);
    border: 2px solid var(--primary-color);
    box-sizing: border-box;
    padding: 20px;
    margin-top: 18px;

    display: flex;
    flex-direction: row;
    align-items: start;
    justify-content: start;
    gap: 50px;
    padding: 50px 20px;
    flex-wrap: wrap;
    align-content: stretch;

    overflow: scroll;

    max-height: 70vi;

  }

  .pill {
    position: absolute;
    width: auto;
    height: auto;
    border-radius: 50px;
    background-color: var(--background-color);
    display: flex;
    gap: 5px;
    flex-direction: row;
    align-items: center;
    justify-content: start;
    padding: 5px 5px;
    margin: 0px 0px 0px 30px;
    z-index: 1;
  }

  .pill .icon {
    position: relative;
    background: url(https://api.iconify.design/carbon:user-avatar-filled.svg) center/cover no-repeat;
    order: -1;
    width: 30px;
    height: 30px;
  }

  .pill .title {
    height: 100%;
    color: var(--primary-color);
    font-family: 'Noto Sans Display';
    font-style: normal;
    font-size: 22px;
    font-weight: 400;
    line-height: 1.0;
    letter-spacing: 0px;
    text-decoration: none;
    text-transform: none;
    padding-right: 5px;
  }
</style>
