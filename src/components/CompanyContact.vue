<template>
  <hr />
  <div class="company-contact">
    <h1 class="contact-title">Contato</h1>
    <h2 class="phone-title">Telefones</h2>
    <p class="company-number">+55 (11) 3088-0757</p>
    <h2 class="email-title">E-mail</h2>
    <p class="company-email">renee@reneetrajar.com.br</p>
    <h2 class="personalized-service">Atendimento Personalizado</h2>
    <button class="button-click-me">Clique aqui!</button>
    <input type="text" placeholder="Nome" class="input-name" />
    <input type="email" placeholder="E-mail" class="input-email" />
    <input type="text" placeholder="Mensagem " class="input-message" />
    <button class="button-send-message">Enviar Mensagem</button>
  </div>
  <footer></footer>
</template>

<script>
export default {
  name: "CompanyContact",
};
</script>

<style scoped>
@import url("http://fonts.googleapis.com/css?family=Lato:400,700");
@import url("https://fonts.googleapis.com/css2?family=Cormorant:ital,wght@0,300;1,300&family=Playfair+Display:ital,wght@0,600;1,400&family=Tajawal:wght@500&family=Work+Sans:ital,wght@0,300;1,700&display=swap");
.company-contact {
  width: 100vw;
  height: 570px;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
}

hr {
  margin: 40px 0;
}

.contact-title {
  font-family: "Cormorant";
  font-style: normal;
  font-weight: 300;
  font-size: 38px;
  line-height: 46px;
  width: 200px;
  height: 50px;
  margin-top: 7%;
  grid-column-start: 2;
  align-items: center;
  text-align: center;

  color: #1c86a4;
}

.phone-title {
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 22px;
  padding-left: 30%;

  text-transform: uppercase;

  color: #1c86a4;

  grid-column-start: 1;
  grid-row-start: 2;
}

.company-number {
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 16px;
  line-height: 150.1%;

  color: #828282;
  padding-left: 30%;
  margin-top: 5%;
  grid-column-start: 1;
  grid-row-start: 2;
}

.email-title {
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 22px;

  text-transform: uppercase;

  color: #1c86a4;
  padding-left: 30%;
  margin-top: 10%;
  grid-column-start: 1;
  grid-row-start: 2;
}

.company-email {
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 16px;
  line-height: 19px;

  color: #828282;
  padding-left: 30%;
  margin-top: 15%;
  grid-column-start: 1;
  grid-row-start: 2;
}

.personalized-service {
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 22px;

  text-transform: uppercase;

  color: #1c86a4;
  padding-left: 30%;
  margin-top: 25%;
  grid-column-start: 1;
  grid-row-start: 2;
}

.button-click-me {
  box-sizing: border-box;

  border: 1px solid #1c86a4;
  border-radius: 2px;

  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 22px;
  width: 270px;
  height: 50px;
  margin-left: 30%;

  text-align: center;

  color: #014561;
  margin-top: 30%;
  grid-column-start: 1;
  grid-row-start: 2;
}

.button-click-me:hover {
  box-sizing: border-box;

  border: 1px solid #be9667;
  color: #be9667;
  border-radius: 2px;
}

.input-name::placeholder,
.input-email::placeholder,
.input-message::placeholder {
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 14px;
  line-height: 17px;

  color: #c4c4c4;
}

.input-name {
  box-sizing: border-box;

  border: 1px solid #1c86a4;
  border-radius: 3px;
  width: 600px;
  height: 42px;
  grid-column-start: 2;
  grid-row-start: 2;
}

.input-email {
  box-sizing: border-box;

  border: 1px solid #1c86a4;
  border-radius: 3px;
  width: 600px;
  height: 42px;
  grid-column-start: 2;
  grid-row-start: 2;
  margin-top: 9%;
}

.input-message {
  box-sizing: border-box;

  border: 1px solid #1c86a4;
  border-radius: 3px;
  width: 600px;
  height: 77px;
  grid-column-start: 2;
  grid-row-start: 2;
  margin-top: 18%;
}

.button-send-message {
  background: #014561;
  border-radius: 2px;
  font-family: "Lato";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 22px;
  width: 600px;
  height: 50px;
  margin-top: 5%;
  grid-column-start: 2;
  grid-row-start: 3;

  text-align: center;

  color: #e5e5e5;
}

.button-send-message:hover {
  background-color: #00648c;
}
</style>
