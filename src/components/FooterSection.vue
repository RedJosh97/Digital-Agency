<template>
  <div class="footer-section">
    <div class="footer-columns">
      <div class="company column">
        <h5>LOREM.IK</h5>
        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        <p>@lorem.lk digital agency</p>
      </div>
      <div class="about column">
        <h5>About us</h5>
        <p>Lorem.IK</p>
        <p>portfolio</p>
        <p>Career</p>
        <p>Contact us</p>
      </div>
      <div class="contact column">
        <h5>Contact us</h5>
        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        <p>+623-1238043848838</p>
      </div>
      <div class="social-handle column">
        <i class="lab la-facebook-f"></i>
        <i class="lab la-instagram"></i>
        <i class="lab la-twitter"></i>
        <i class="lab la-linkedin-in"></i>
      </div>
    </div>
    <p class="copyright">2023 vue project</p>
  </div>
</template>

<script>
export default {
  name: 'FooterSection'
}
</script>

<style scoped>
.footer-section {
  background: #040844;
  color: #fff;
  padding: 3em 6em 1em;
}

.footer-section p {
  font-size: 10px;
}

.copyright {
  text-align: center;
}
.column {
  align-items: flex-end;
}
.column p {
  font-size: 12px;
}

.about {
  width: 220px;
}

.footer-columns {
  display: flex;
  gap: 40px;
  margin-bottom: 3em;
}

.social-handle {
  display: flex;
  gap: 7px;
}

.lab {
  padding: 2px;
  color: #040844;
  background: #fff;
  border-radius: 50px;
}

@media (max-width: 790px) {
  .footer-columns {
    display: grid;
    grid-template-columns: 240px 100px;
    justify-content: space-between;
    justify-items: self-end;
  }

  .about {
    text-align: right;
    width: 120px;
  }
}

@media (max-width: 580px) {
  .footer-columns {
    text-align: center;
    display: flex;
    justify-content: center;
    flex-direction: column;
    gap: 12px;
  }
  .about {
    margin: 0 auto;
    text-align: center;
  }
  .social-handle {
    margin: 0 auto;
    text-align: center;
  }
}
</style>
