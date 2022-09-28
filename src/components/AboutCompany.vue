<template>
  <div class="div-about-company">
    <img :src="image" id="image-renee" />
    <h2 class="name-renee">Renee Trajar</h2>
    <p class="first">
      Com mais de 35 anos de experiência em camisas, calças e ternos sob medida,
      possuímos profissionais experientes e altamente qualificados.
    </p>
    <p class="second">
      Cada cliente tem seu molde exclusivamente desenvolvido para seu biotipo
      através das medidas tiradas pelo próprio Sr. Renee, no escritório ou
      residência do cliente.
    </p>
    <p class="third">
      “Nosso objetivo é superar a expectativa do cliente proporcionando-lhe
      satisfação ao usar nossos produtos, aliado a um relacionamento franco e
      honesto, valorizando o ser humano.”
    </p>
    <p class="autor-phrase">Renee Trajar</p>
    <button>Agende uma visita!</button>
  </div>
</template>

<script>
export default {
  name: "AboutCompany",
  data() {
    return {
      image: require("@/assets/imgs-aboutCompany/renee.png"),
    };
  },
};
</script>

<style scoped>
@import url("http://fonts.googleapis.com/css?family=Lato:400,700");
@import url("https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;1,300&family=Playfair+Display:ital,wght@0,600;1,400&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
.div-about-company {
  width: 100vw;
  height: 570px;
  left: 0px;
  background-color: rgb(255, 255, 255);
  display: grid;
  grid-template-columns: 0.5fr 1.5fr 0.5fr 0.5fr;
  grid-template-rows: 1fr 1fr 1fr;
}

#image-renee {
  grid-column-start: 1;
  grid-column-end: 3;
  grid-row-start: 2;
  grid-row-end: 3;
  padding-left: 90px;
}

.name-renee {
  height: 46px;
  left: 55%;
  margin: 0;

  font-family: "Cormorant";
  font-style: normal;
  font-weight: 300;
  font-size: 38px;
  line-height: 46px;

  display: flex;
  align-items: center;
  text-align: center;

  color: #014561;

  grid-column-start: 3;
  grid-column-end: 3;
  grid-row-start: 2;
  grid-row-end: 3;
}

.first {
  width: 700px;
  height: 135px;
  margin-top: 10%;

  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 19px;
  line-height: 141.3%;

  color: #333333;
  grid-column-start: 3;
  grid-column-end: 4;
  grid-row-start: 2;
  grid-row-end: 3;
}

.second {
  width: 700px;
  height: 135px;
  margin-top: 20%;

  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 19px;
  line-height: 141.3%;

  color: #333333;
  grid-column-start: 3;
  grid-column-end: 4;
  grid-row-start: 2;
  grid-row-end: 3;
}

.third {
  width: 678px;
  height: 102px;
  margin-top: 30%;

  font-family: "Cormorant";
  font-style: italic;
  font-weight: 400;
  font-size: 24px;
  line-height: 141.3%;

  color: #1c86a4;
  grid-column-start: 3;
  grid-column-end: 4;
  grid-row-start: 2;
  grid-row-end: 3;
}

button {
  width: 300px;
  height: 50px;
  margin-top: 50%;

  background: #014561;
  border-radius: 2px;

  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 22px;

  place-items: center;

  text-align: center;

  color: #e5e5e5;
  grid-column-start: 3;
  grid-column-end: 3;
  grid-row-start: 2;
  grid-row-end: 3;
}

.autor-phrase {
  width: 101px;
  height: 28px;
  margin-left: 80%;
  margin-top: 43%;
  font-family: "Cormorant";
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 141.3%;

  color: #828282;
  grid-column-start: 3;
  grid-column-end: 4;
  grid-row-start: 2;
  grid-row-end: 3;
}

.sublinhado-gradiente:hover {
  background-image: linear-gradient(90deg, red, blue);
  background-repeat: no-repeat;
  background-size: 0% 3px;
  background-position: left bottom;
  transition: background-size 500ms ease;
  cursor: pointer;
  text-decoration: none;
  font-weight: 900;
}
</style>
