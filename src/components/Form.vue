<template>
  <form class="form" action="" method="">

    <fieldset>
      <legend>Nombre <span>*</span></legend>
      <input
        id="name"
        name="name"
        type="text"
        placeholder="Nombre"
      >
    </fieldset>

    <fieldset>
      <legend>Email <span>*</span></legend>
      <input
        id="email"
        name="email"
        type="email"
        placeholder="yourmail@gmail.com"
      >
    </fieldset>

    <fieldset>
      <legend>Mensaje <span>*</span></legend>
      <textarea
        id="message"
        name="message"
        placeholder="Tu mensaje"
      ></textarea>
    </fieldset>

    <input class="submit" type="submit" value="Enviar">

  </form>
</template>

<script>
export default {
  name: 'Form',

  data() {
    return {
    }
  },

  methods: {
  },

  mounted() {
  }
}
</script>

<style scoped>

.form {
  background-color: var(--surface);

  border: 1px solid var(--border);
  border-radius: 15px;

  display: flex;
  flex-direction: column;

  gap: 20px;

  padding: 50px;
}

/* Cada campo */
fieldset {
  width: 100%;
  min-width: 0;
  box-sizing: border-box;

  border: 1px solid var(--border);
  border-radius: 6px;

  margin: 0;
  padding: 0 12px 10px;
}

/* Título que queda encima del borde */
legend {
  padding: 0 6px;
  margin-left: 5px;

  font-size: 13px;
  color: #333;
}

/* Asterisco rojo */
legend span {
  color: red;
}

/* Input y textarea */
input,
textarea {
  display: block;

  width: 100%;
  box-sizing: border-box;

  border: none;
  outline: none;

  background: transparent;

  padding: 8px 0;

  font-family: inherit;
  font-size: 14px;
}

/* Textarea */
textarea {
  height: 100px;
  resize: none;
}

/* Botón */
.submit {
  width: 100%;

  padding: 12px;

  border: none;
  border-radius: 6px;

  background-color: #5bb3b5;
  color: white;

  font-size: 20px;
  font-weight: bold;

  cursor: pointer;
}

.submit:hover {
  opacity: 0.9;
}

</style>