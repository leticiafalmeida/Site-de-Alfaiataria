<template>
  <NavBar />
  <AboutCompany />
  <CommentGarey />
  <CompanyPromotion />
  <CompanyProducts />
  <CompanyContact />
  <PageFooter />
</template>

<script>
import NavBar from "./components/NavBar.vue";
import AboutCompany from "./components/AboutCompany.vue";
import CommentGarey from "./components/CommentGarey.vue";
import CompanyPromotion from "./components/CompanyPromotion.vue";
import CompanyProducts from "./components/CompanyProducts.vue";
import CompanyContact from "./components/CompanyContact.vue";
import PageFooter from "./components/PageFooter.vue";
export default {
  name: "App",
  components: {
    NavBar,
    AboutCompany,
    CommentGarey,
    CompanyPromotion,
    CompanyProducts,
    CompanyContact,
    PageFooter,
  },
};
</script>

<style>
body {
  overflow-x: hidden;
}
</style>
