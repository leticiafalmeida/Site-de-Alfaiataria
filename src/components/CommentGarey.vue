<template>
  <div class="comment-garey">
    <div class="background-image">
      <img :src="image1" id="background-image" />
    </div>
    <p class="first">
      “Faço roupas com o Renee Trajar há mais de duas décadas, o serviço é
      impecável em todos os detalhes, desde a costura ao caimento. O Renee tem
      uma equipe de mestre!”
    </p>
    <h2 class="name-autor">Nelson Garey</h2>
    <p class="profission">Advogado | Nelson Garey Advogados Associados</p>
    <img :src="image2" id="background-image2" />
    <div class="image3"></div>
  </div>
</template>

<script>
export default {
  name: "CommentGarey",
  data() {
    return {
      image1: require("@/assets/imgs-commentG/background.png"),
      image2: require("@/assets/imgs-commentG/garey.png"),
    };
  },
};
</script>

<style scoped>
@import url("http://fonts.googleapis.com/css?family=Lato:400,700");
@import url("https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;1,300&family=Playfair+Display:ital,wght@0,600;1,400&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
.comment-garey {
  width: 100vw;
  height: 360px;
  left: 0%;
  top: 205%;
  background-color: #fff;
  display: grid;
  grid-template-columns: 0.5fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
}

.image3 {
  width: 313px;
  height: 360px;

  grid-column-start: 4;
  grid-column-end: 4;
  grid-row-start: 1;
  grid-row-end: 2;

  background: linear-gradient(rgba(2, 75, 104, 0.81), rgba(2, 75, 104, 0.81)),
    url(@/assets/imgs-commentG/gareySentado.png) no-repeat;
}

.background-image {
  margin-left: 12%;
  grid-column-start: 2;
  grid-column-end: 3;
  grid-row-start: 1;
  grid-row-end: 2;
}

#background-image2 {
  width: 260px;
  height: 310px;
  border: 8px solid #ffffff;
  box-sizing: border-box;
  margin-left: 86%;
  margin-top: 22px;

  filter: drop-shadow(0px 4px 20px rgba(0, 0, 0, 0.25));
  transform: rotate(10deg);

  grid-column-start: 2;
  grid-column-end: 3;
  grid-row-start: 1;
  grid-row-end: 2;
  z-index: 1;
}

.first {
  width: 630px;
  height: 102px;
  margin-left: 15%;
  margin-top: 5%;

  font-family: "Lato";
  font-style: normal;
  font-weight: 100;
  font-size: 24px;
  line-height: 141.3%;

  text-align: center;

  color: #828282;
  grid-column-start: 2;
  grid-column-end: 3;
  grid-row-start: 1;
  grid-row-end: 2;
}

.name-autor {
  width: 200px;
  height: 40px;
  margin-left: 40%;
  margin-top: 23%;

  font-family: "Cormorant";
  font-style: italic;
  font-weight: 400;
  font-size: 28px;
  line-height: 141.3%;

  text-align: center;

  color: #014561;
  grid-column-start: 2;
  grid-column-end: 3;
  grid-row-start: 1;
  grid-row-end: 2;
}

.profission {
  width: 425px;
  height: 28px;
  margin-left: 27%;
  margin-top: 27%;

  font-family: "Lato";
  font-style: normal;
  font-weight: 100;
  font-size: 20px;
  line-height: 141.3%;

  text-align: center;

  color: #be9667;
  grid-column-start: 2;
  grid-column-end: 3;
  grid-row-start: 1;
  grid-row-end: 2;
}
</style>
