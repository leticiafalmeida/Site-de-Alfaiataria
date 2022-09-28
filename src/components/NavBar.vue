<template>
  <div class="nav-bar">
    <header class="header">
      <h2 class="logo" href="/">Renne Trajar</h2>
      <img :src="image" class="logo-image" />
      <nav>
        <ul class="options">
          <li><a href="/">Empresa</a></li>
          <li><a href="/">Camisaria</a></li>
          <li><a href="/">Alfaitaria</a></li>
          <li><a href="/">Depoimentos</a></li>
          <li><a href="/">Contato</a></li>
        </ul>
      </nav>
    </header>
    <p class="first-phrase">Elegante é ter um</p>
    <p class="alfaiate-title">alfaiate</p>
    <p class="second-phrase">para chamar de seu.</p>
    <p class="promotion">
      COMPRE HOJE, PAGUE EM ATÉ 3X COM 12% DE DESCONTO E TENHA 10 MESES PARA
      CONFECCIONAR!
    </p>
    <button class="button-budget">FAÇA JÁ UM ORÇAMENTO</button>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      image: require("@/assets/imgs-navBar/logo.png"),
    };
  },
};
</script>

<style scoped>
@import url("http://fonts.googleapis.com/css?family=Lato:400,700");
@import url("https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,600;1,400&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;1,300&family=Playfair+Display:ital,wght@0,600;1,400&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
.nav-bar {
  width: 100vw;
  height: 625px;
  left: 0px;
  top: 0%;
  background-image: url(@/assets/imgs-navBar/background.png);
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
}

.logo {
  font-size: 25px;
  letter-spacing: 5px;
  font-family: "Cormorant";
  color: white;
  width: 100px;
  font-weight: 100;
  padding-left: 40%;
  padding-top: 5%;
  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 1;
  z-index: 1;
}

.logo-image {
  left: 2.93%;
  right: 95.23%;
  top: 0.55%;
  bottom: 98.47%;
  padding-left: 28%;
  margin-top: 40px;

  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 1;
}

a {
  color: #949494;
  transition: 0.3s;
  text-transform: uppercase;
  font-size: 16px;
  font-weight: 300;
  text-decoration: none;
  padding-right: 50px;
}

a:hover {
  color: #007a9b;
}

header {
  position: fixed;
  width: 100vw;
  background: linear-gradient(180deg, #000000 29.73%, rgba(0, 0, 0, 0) 100%);
  display: grid;
  grid-template-columns: 1fr 1fr;
  z-index: 1;
  margin-top: -15px;
  margin-left: -15px;
}

nav {
  display: flex;
  justify-content: space-around;
  font-family: "Lato";
  height: 8vh;

  padding: 30px;

  grid-row-start: 1;
  grid-column-start: 3;
  z-index: 1;
}

.options {
  list-style: none;
  display: flex;
}

.options li {
  margin-left: 5px;
}

.first-phrase {
  width: 348.69px;
  height: 43.05px;
  margin-top: 30%;

  margin-left: 22%;

  font-family: "Playfair Display";
  font-style: italic;
  font-weight: 400;
  font-size: 32.5627px;
  line-height: 43px;

  color: #be9667;

  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 1;
  grid-row-end: 2;
}

.alfaiate-title {
  width: 404.18px;
  height: 119.58px;
  margin-left: 20%;
  margin-top: 35%;
  font-family: "Playfair Display";
  font-style: normal;
  font-weight: 400;
  font-size: 90.0346px;
  line-height: 120px;

  text-transform: uppercase;

  color: rgba(2, 75, 104, 0.68);

  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 1;
  grid-row-end: 2;
}

.second-phrase {
  width: 289px;
  height: 43px;
  margin-left: 50%;
  margin-top: 58%;

  font-family: "Playfair Display";
  font-style: italic;
  font-weight: 400;
  font-size: 32.5627px;
  line-height: 43px;

  color: #be9667;

  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 1;
  grid-row-end: 2;
}

.promotion {
  width: 438px;
  height: 93px;
  margin-top: 10%;
  margin-left: 20%;
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 24px;
  line-height: 131%;
  color: #e5e5e5;
  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 2;
  grid-row-end: 3;
}

.button-budget {
  margin-left: 20%;
  margin-top: 5%;

  width: 297px;
  height: 50px;
  font-family: "Lato";
  font-style: normal;
  font-weight: 100;
  font-size: 18px;
  color: #e5e5e5;

  background: #014561;
  border-radius: 2px;
  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-start: 3;
  grid-row-end: 3;
}
.button-budget:hover {
  border-color: #be9667;
  background: #000000;
  color: #ccc;
}
</style>
