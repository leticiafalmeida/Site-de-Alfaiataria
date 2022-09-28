<template>
  <div class="company-promotion">
    <img :src="image" id="promotion" />

    <h1 class="title">Condição Imperdível</h1>
    <h2 class="subtitle">Compre hoje e garanta:</h2>
    <ul class="description">
      <li>12% de desconto e pagamento em até 3x sem juros;</li>
      <li>
        Até 10 meses para confeccionar sua roupa. Não se preocupe se suas
        medidas aumentaram ou diminuíram, estará sempre elegante;
      </li>
      <li>Condição muito especial por tempo limitado;</li>
      <li>Poder presentear alguém com uma roupa de alta costura, exclusiva.</li>
    </ul>

    <button>Garanta essa condição especial!</button>
  </div>
</template>

<script>
export default {
  name: "CompanyPromotion",
  data() {
    return {
      image: require("@/assets/imgs-promotion/promotion.png"),
    };
  },
};
</script>

<style scoped>
@import url("http://fonts.googleapis.com/css?family=Lato:400,700");
@import url("https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,600;1,400&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;1,300&family=Playfair+Display:ital,wght@0,600;1,400&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
.company-promotion {
  width: 100vw;
  height: 570px;
  display: grid;
  grid-template-columns: 0.5fr 1.5fr 1fr;
  grid-template-rows: 1fr 1fr;

  background: linear-gradient(
      rgba(1, 49, 69, 0.839) 0%,
      rgba(0, 36, 50, 0.963) 0%
    ),
    url(@/assets/imgs-promotion/backpromotion.png) no-repeat;
}

#promotion {
  grid-column-start: 3;
  grid-row-start: 1;
  margin-top: 25px;
  padding-left: 30px;
}

.title {
  font-family: "Cormorant";
  font-style: normal;
  font-weight: 400;
  font-size: 53px;
  line-height: 64px;
  text-transform: uppercase;
  margin-top: 35px;
  grid-row-start: 1;
  grid-column-start: 2;

  height: 55px;

  color: #be9667;

  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}

.subtitle {
  font-family: "Cormorant";
  font-style: italic;
  font-weight: 400;
  font-size: 30px;
  line-height: 36px;
  height: 55px;
  margin-top: 125px;

  grid-column-start: 2;
  grid-row-start: 1;

  color: #be9667;

  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}

.description {
  font-family: "Lato";
  font-style: normal;
  font-weight: 100;
  font-size: 22px;
  line-height: 26px;
  height: 250px;
  grid-column-start: 2;
  grid-row-start: 1;
  margin-top: 30%;

  color: #c4c4c4;
}

.description li {
  list-style-image: url("@/assets/imgs-products/traco.png");
  margin-bottom: 12px;
}

button {
  width: 330px;
  height: 55px;
  background: #be9667;
  border-radius: 3px;
  font-family: "Lato";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 22px;
  grid-column-start: 2;
  grid-row-start: 1;
  margin-top: 65%;

  text-align: center;

  color: #e0e0e0;
}

button:hover {
  background: #727272;
  outline: none;
}
</style>
