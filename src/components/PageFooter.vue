<template>
  <hr />
  <footer>
    <img :src="image" class="logo-image" />
    <h2 class="logo" href="/">Renne Trajar</h2>
    <h2 class="tag-line">Camisaria e Alfaitaria</h2>
    <p class="copy-right">
      Copyright: 2021 © Renee Trajar - Todos os direitos reservados.
    </p>
    <p class="cnpj">CNPJ:04.487.685/0001-01</p>
  </footer>
</template>

<script>
export default {
  name: "PageFooter",
  data() {
    return {
      image: require("@/assets/imgs-navBar/logo.png"),
    };
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;1,300&family=Playfair+Display:ital,wght@0,600;1,400&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;1,300&family=Playfair+Display:ital,wght@0,600;1,400&family=Poppins:wght@200&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
footer {
  display: grid;
  grid-template-columns: 1fr 1fr;
  width: 100vw;
  height: 200px;
}

.logo {
  font-size: 35px;
  letter-spacing: 8px;
  font-family: "Cormorant";
  color: black;
  width: 70px;
  font-weight: bold;
  padding-left: 25%;
  margin-top: 23px;
  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 1;
}

.tag-line {
  font-size: 12px;
  font-family: "Cormorant";
  color: black;
  font-weight: bold;
  width: 190px;
  height: 50px;
  padding-left: 26%;
  margin-top: 105px;
  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 1;
  white-space: nowrap;
}

.logo-image {
  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 1;
  padding-left: 20%;
  margin-top: 50px;
}

.cnpj {
  width: 170px;
  height: 23px;

  font-family: "Poppins";
  font-style: normal;
  font-weight: 300;
  font-size: 14px;
  line-height: 21px;

  padding-left: 22%;
  margin-top: -20px;

  color: #bdbdbd;
  grid-column-start: 1;
  grid-column-end: 1;
  white-space: nowrap;
}

.copy-right {
  width: 426px;
  height: 23px;
  margin-top: -10px;

  font-family: "Poppins";
  font-style: normal;
  font-weight: 300;
  font-size: 14px;
  line-height: 21px;
  text-align: center;
  grid-column-start: 2;
  grid-row-start: 2;

  /* Gray 2 */

  color: #4f4f4f;
}
</style>
