<template>
  <div class="sectionSide">
    <div class="text-side">
      <p>Truested Client</p>
      <h4>Lorem Ipsum is simply dummy text dummy text</h4>
    </div>
    <div class="company">
      <img src="/image/354-3549351_client-earth-logo.png" />
      <img src="/image/biotechne+logo-1.png" />
      <img src="/image/biotechne+logo.png" />
      <img src="/image/clientlogo-8-3.png" />
      <img src="/image/Inmarc-client-logos-Recovered-32.png" />
      <img src="/image/Kudos-Client-Logo-3.png" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'SectionSide'
}
</script>

<style scoped>
.sectionSide {
  background: #fcfcfc;
  padding: 5em 6em;
}

.text-side {
  text-align: center;
  font-family: Poppins;
  font-size: 17px;
  margin: 0 auto;
}
.text-side p {
  color: #767676;
  margin-bottom: 1.2em;
}
.text-side h4 {
  color: #000;
}

.company {
  padding-top: 2.5em;
  justify-content: space-between;
  display: flex;
  align-items: center;
}
.company img {
  width: 120px;
  min-width: 30px;
}

@media (max-width: 884px) {
  .sectionSide {
    padding-top: 20em;
  }
}

@media (max-width: 700px) {
  .sectionSide {
    padding: 20em 1.7em 0;
  }
}
</style>
