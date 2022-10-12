<template>
  <div class="contacto">
    <div class="title">
      <h2>CONTACTO</h2>
    </div>
    <div class="formulario">
      <input type="text" placeholder="NOMBRE" />
      <input type="email" placeholder="CORREO" />
      <input type="text" placeholder="CELULAR" />
      <textarea name="" placeholder="MENSAJE" cols="30" rows="10"></textarea>
      <button>ENVIAR</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.contacto {
  padding: 2rem 0;
}

.contacto .title {
  width: 12rem;
  border: 8px solid #000000;
  margin: 0 auto;
}

.contacto .formulario {
  margin: 2rem auto 0 auto;
  width: 40%;
  display: flex;
  flex-direction: column;
}

.contacto .formulario input {
  margin: 0.5rem 0;
  padding: 0.5rem;
  border-left: 2.5px solid #000000;
  border-right: none;
  border-top: none;
  border-bottom: 2.5px solid #000000;
  background: transparent;
  outline: none;
  font-family: "Roboto";
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 17px;
  display: flex;
  align-items: center;
  letter-spacing: 0.04em;
}

.contacto .formulario input::placeholder {
  color: #8b8b8b;
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 17px;
  display: flex;
  align-items: center;
  letter-spacing: 0.04em;
}

.contacto .formulario textarea {
  margin: 0.5rem 0;
  padding: 0.5rem;
  border-left: 3px solid #000000;
  border-right: none;
  border-top: none;
  border-bottom: 3px solid #000000;
  background: transparent;
  outline: none;
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 17px;
  display: flex;
  align-items: center;
  letter-spacing: 0.04em;
}

.contacto .formulario textarea::placeholder {
  color: #8b8b8b;
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 17px;
  display: flex;
  align-items: center;
  letter-spacing: 0.04em;
}

.contacto .formulario button {
  width: 8rem;
  height: 2.4rem;
  margin: 2rem auto 0 auto;
  border-right: 3px solid #000000;
  border-left: 3px solid #000000;
  border-top: none;
  border-bottom: none;
  font-weight: bold;
  cursor: pointer;
  background: transparent;
}

.contacto .formulario button:hover {
  background: #000000;
  color: #ffffff;
}

@media screen and (max-width: 768px) {
  .contacto .formulario {
    width: 75%;
  }
}
</style>
