<template>
  <div class="outro_page">
    <div class="banners">
      <img src="../assets/banner_1.png" />
      <img src="../assets/banner_2.png" />
    </div>
    <div class="content">
      <img src="../assets/About_us.svg" />
      <h2>World Best Travel Agency Company Since 2008.</h2>
      <p>
        Continually productize compelling quality for packed with elated productize
        compelling quality for packed in with all elated Them Setting up to website and
        creating pages.
      </p>
      <ul>
        <li>We providing compe quality for packed with elated different.</li>
        <li>We are one of compelling quality for packed with leading.</li>
        <li>Learn how compelling quality for packed with elated grow.</li>
      </ul>
      <div class="facts">
        <div class="fact">
          <h3>20+</h3>
          <p>Year exprerience</p>
        </div>
        <div class="fact">
          <h3>250+</h3>
          <p>Destination collaboration</p>
        </div>
        <div class="fact">
          <h3>170K+</h3>
          <p>Happy customers</p>
        </div>
      </div>
      <button>Read more</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "OutroPage",
};
</script>

<style lang="scss">
.outro_page {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  max-width: 1320px;
  margin: 50px auto;

  .banners {
    position: relative;
    width: 580px;
    height: 580px;
    img:first-child {
      z-index: 1;
      height: 520px;
      width: 410px;
    }
    img:last-child {
      position: absolute;
      right: 0;
      bottom: 0;
      z-index: 2;
      height: 280;
      width: 265px;
    }
  }
  .content {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: space-between;
    height: 540px;
    width: 525px;

    img {
      width: 90;
      height: 16px;
    }
    h2 {
      color: #1f3347;
      line-height: 1.3em;
      font-weight: 600;
      font-size: 36px;
    }
    p {
      font-size: 16px;
      color: #9da1b4;
    }
    ul {
      padding: 0 10px;
      li {
        font-size: 16px;
        color: #9da1b4;
        margin: 10px 0;
      }
    }
    .facts {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 10px;
      width: 100%;
      .fact {
        max-width: 80px;
        h3 {
          color: #ffc814;
          font-size: 36px;
        }
        p {
          margin-top: 5px;
          font-size: 16px;
          line-height: 1.5em;
          color: #9da1b4;
        }
      }
    }
    button {
      width: 160px;
      height: 45px;
      font-size: 16px;
      background-color: #ffc814;
      border-radius: 4px;
    }
  }
}
</style>
