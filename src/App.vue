<template class="appFile">
  <NavBar />
  <HeroSection />
  <SectionSide />
  <ProductItem />
  <BusinessArticle />
  <WorkDialogue />
  <TestimonialSection />
  <LatestNews />
  <FooterSection />
</template>

<script>
import WorkDialogue from './components/WorkDialogue.vue'
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import SectionSide from './components/SectionSide.vue'
import ProductItem from './components/ProductItem.vue'
import BusinessArticle from './components/BusinessArticle.vue'
import TestimonialSection from './components/TestimonialSection.vue'
import LatestNews from './components/LatestNews.vue'
import FooterSection from './components/FooterSection.vue'
export default {
  name: 'app',
  components: {
    NavBar,
    HeroSection,
    SectionSide,
    ProductItem,
    BusinessArticle,
    TestimonialSection,
    LatestNews,
    FooterSection,
    WorkDialogue
  }
}
</script>
