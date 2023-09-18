<template>
  <div class="navContainer">
    <div class="navBar">
      <div>
        <h1>Logo</h1>
      </div>
      <div class="logos">
        <i class="lab la-facebook-f"></i>
        <i class="lab la-instagram"></i>
        <i class="lab la-twitter"></i>
        <i class="lab la-linkedin-in"></i>
      </div>
    </div>
    <button class="contact">Contact us</button>
  </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style scoped>
.navContainer {
  display: flex;
}
.navBar {
  background-color: #fff;
  height: 50px;
  width: calc(100vw - 180px);
  padding: 0.5em 3em;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.navBar h1 {
  color: #282c6d;
  font-family: Poppins;
  font-size: 38px;
  font-style: normal;
  font-weight: 600;
  width: 20vw;
  line-height: normal;
}
.logos {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
}

.logos .lab {
  background: white;
  filter: drop-shadow(0px 4px 14px rgba(0, 0, 0, 0.15));
  font-size: 16px;
  padding: 12px;
  border-radius: 50%;
  gap: 12px;
}

.logos button {
  margin-left: 2em;
}

.contact {
  background: linear-gradient(123deg, #ffd910 -22.55%, #ffca10 121.01%);
  width: 180px;
  color: #282c6d;
  font-size: 19px;
  border: none;
  border-radius: 0 0 12px 12px;
}

@media (max-width: 570px) {
  .logos {
    display: none;
  }
}
</style>
