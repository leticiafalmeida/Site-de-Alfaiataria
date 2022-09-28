<template>
  <div class="company-products">
    <div class="image-shirt"><img :src="imageShirt" /></div>

    <div class="box-shirt">
      <h1 class="shirt-title">Camisaria</h1>
      <li class="shirt-subtitle">confeccionadas artesanalmente</li>
      <ul class="shirt-description1">
        <li>100% Algodão</li>
        <li>Monograma</li>
        <li>Slim</li>
      </ul>
      <ul class="shirt-description2">
        <li>Nacionais e Importadas</li>
        <li>Tradicionais e Esportivas</li>
        <li>Casamentos</li>
      </ul>
      <div class="shirt-square"></div>
      <button class="shirt-button">Quero um orçamento</button>
    </div>

    <img :src="imageSuit" class="image-suit" />
    <div class="box-suit">
      <h1 class="suit-title">Alfaiataria</h1>
      <li class="suit-subtitle">totalmente feito a mão sob medida</li>
      <ul class="suit-description1">
        <li>Fio Super 120 e 130</li>
        <li>Lã fria Australiana</li>
        <li>Botões Importados</li>
      </ul>
      <ul class="suit-description2">
        <li>Ternos e Calças</li>
        <li>Paletós e Smokings</li>
        <li>Sociais e Esportivos</li>
      </ul>
      <div class="suit-square"></div>

      <button class="suit-button">Quero um orçamento</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "CompanyProducts",
  data() {
    return {
      imageShirt: require("@/assets/imgs-products/camisaria.png"),
      imageSuit: require("@/assets/imgs-products/alfaiataria.png"),
    };
  },
};
</script>

<style scoped>
@import url("http://fonts.googleapis.com/css?family=Lato:400,700");
@import url("https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;1,300&family=Playfair+Display:ital,wght@0,600;1,400&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
.company-products {
  width: 100vw;
  height: 230vh;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr 1fr;
}

.image-shirt {
  margin-top: 195px;
  margin-left: 150px;
  position: absolute;
}

.image-suit {
  grid-row-start: 3;
  grid-column-start: 2;
  margin-left: -350px;
  margin-top: 10%;
  z-index: 1;
}

.shirt-square {
  width: 550px;
  height: 464px;
  z-index: 1;
  box-sizing: border-box;
  border: 1px solid #1c86a4;
  grid-column-start: 1;
  margin: 0px;
  margin-left: -112px;
  margin-top: -290px;
}

.suit-square {
  width: 550px;
  height: 464px;
  z-index: 1;
  box-sizing: border-box;
  border: 1px solid #1c86a4;
  grid-column-start: 2;
  margin: 0px;
  margin-left: 148px;
  margin-top: -220px;
}

.box-shirt {
  box-sizing: border-box;
  border: 1px solid #e5e5e5;
  width: 1001px;
  height: 395px;
  margin-left: 25%;
  margin-top: 25%;
  display: grid;
  grid-template-columns: 1fr 1fr;
}

.box-suit {
  box-sizing: border-box;
  border: 1px solid #e5e5e5;
  grid-row-start: 3;
  grid-column-start: 1;
  width: 1001px;
  height: 395px;
  margin-left: 10%;
  margin-top: 80px;
  display: grid;
  grid-template-columns: 1fr 1fr;
}

.shirt-title {
  font-family: "Cormorant";
  font-style: normal;
  font-weight: 300;
  font-size: 62px;
  line-height: 75px;
  grid-column-start: 2;
  margin-top: -5px;

  text-transform: uppercase;

  color: #014561;
}

.suit-title {
  font-family: "Cormorant";
  font-style: normal;
  font-weight: 300;
  font-size: 62px;
  line-height: 75px;
  margin-left: 15%;
  margin-top: 10px;
  grid-column-start: 1;

  text-transform: uppercase;

  color: #014561;
}

.shirt-subtitle {
  font-family: "Lato";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 19px;
  text-transform: uppercase;
  grid-column-start: 2;
  height: 50px;

  color: #c4c4c4;

  list-style-image: url("@/assets/imgs-products/traco.png");
  margin-top: -55px;
}

.suit-subtitle {
  font-family: "Lato";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 19px;
  margin-left: 15%;
  text-transform: uppercase;
  grid-column-start: 1;
  height: 20px;
  margin-top: -40px;

  color: #c4c4c4;

  list-style-image: url("@/assets/imgs-products/traco.png");
}

.shirt-description1 {
  width: 180px;
  height: 100px;
  grid-column-start: 2;
  margin-top: -35px;
}

.suit-description1 {
  width: 200px;
  height: 60px;
  grid-column-start: 1;
  margin-left: 15%;
  margin-top: -10px;
}

.shirt-description2 {
  width: 270px;
  height: 100px;
  grid-column-start: 2;
  margin-top: -32px;
}

.suit-description2 {
  width: 270px;
  height: 100px;
  grid-column-start: 1;
  margin-left: 12%;
}

.shirt-description1 li,
.shirt-description2 li {
  font-family: "Cormorant";
  font-style: italic;
  font-weight: 400;
  font-size: 24px;
  line-height: 29px;
  grid-column-start: 2;
  color: #727272;
}

.suit-description1 li,
.suit-description2 li {
  font-family: "Cormorant";
  font-style: italic;
  font-weight: 400;
  font-size: 24px;
  line-height: 29px;
  grid-column-start: 1;
  margin-left: 15%;
  color: #727272;
  width: 200px;
}

.shirt-button {
  background: #014561;
  border-radius: 2px;
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 22px;
  grid-column-start: 2;
  width: 330px;
  height: 50px;
  text-align: center;
  margin-top: -15px;

  color: #e5e5e5;
}

.shirt-button:hover,
.suit-button:hover {
  background: #013145;
  transition: 0.5s;
}

.suit-button {
  background: #014561;
  border-radius: 2px;
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 22px;
  grid-column-start: 1;
  width: 330px;
  height: 50px;
  text-align: center;
  margin-top: -120px;
  margin-left: 15%;

  color: #e5e5e5;
}
</style>
