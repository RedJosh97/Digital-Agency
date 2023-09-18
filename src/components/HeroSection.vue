<template>
  <div class="headerContainer">
    <div class="headerBox">
      <div class="headerDetails">
        <h5>We deliver <span>Superb Creative</span> Output to make great things happen.</h5>
        <p>
          Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has
          been the industry's standard dummy text ever
        </p>
        <button>Let's get start</button>
      </div>

      <div>
        <img src="/image/meeting.png" class="meetingPic" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeroSection'
}
</script>

<style scoped>
.headerContainer {
  background: #fcfcfc;
  height: calc(100vh - 67px);
  display: flex;
  padding: 0 6em;
}
.headerBox {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
}
.headerDetails h5 {
  color: #000;
  font-family: Poppins;
  font-size: 1.8em;
  font-weight: 500;
  line-height: 40px;
}

span {
  color: #04b200;
  font-family: Poppins;
  font-size: 1em;
  font-weight: 600;
  line-height: 50px;
}
.headerDetails p {
  margin-top: 22px;
  color: #9a9a9a;
  font-family: Poppins;
  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  line-height: 31px;
}

.meetingPic {
  width: 10%;
  min-width: 100%;
}

.headerDetails {
  width: 520px;
  display: flex;
  justify-content: center;
  flex-direction: column;
}
.headerDetails button {
  margin-top: 2em;
  width: 150px;
  height: 37px;
  color: #fff;
  border: none;
  font-family: Poppins;
  font-size: 13px;
  border-radius: 7px;
  background: #282c6d;
  box-shadow: 0px 8px 34px 0px rgba(40, 44, 109, 0.31);
}

@media only screen and (max-width: 884px) {
  .headerBox {
    display: flex;
    flex-direction: column;
    margin: 30px auto;
  }
  .headerDetails {
    width: 100%;
    font-size: 1em;
  }

  .headerDetails p {
    font-size: 18px;
    line-height: 22px;
  }
  .headerDetails h5 span {
    line-height: 2 px;
  }
  .headerDetails button {
    margin: 0 auto;
    margin-top: 3em;
  }

  .meetingPic {
    /* width: 230px; */
    height: auto;
  }
}
@media (max-width: 700px) {
  .headerContainer {
    padding: 1.7em;
  }
}
</style>
