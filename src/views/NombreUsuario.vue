<template>
    <div>
      <h2>Ingresar Nombre de Usuario</h2>
      <form @submit="submitForm">
        <label for="username">Nombre de usuario:</label>
        <input
          id="username"
          type="text"
          v-model="username"
          :maxlength="8"
          pattern="[a-zA-Z]+"
          required
        />
        <button type="submit">Guardar</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        username: '',
      };
    },
    methods: {
      submitForm(event) {
        event.preventDefault();
        // Validar el nombre de usuario
        if (/[^0-9a-zA-Z]/.test(this.username)) {
          alert('El nombre de usuario no puede contener números ni caracteres especiales.');
          return;
        }
        if (this.username.length > 8) {
          alert('El nombre de usuario debe tener máximo 8 caracteres.');
          return;
        }
        // Guardar el nombre de usuario para utilizar en otras vistas
        this.$store.commit('setUsername', this.username);
        // Redirigir a otra vista
        this.$router.push('/otra-vista');
      },
    },
  };
  </script>