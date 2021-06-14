<template>
  <div class="registro">
    <v-card elevation="3">
      <v-form class="form form--registro pa-10" @submit.prevent='registrarCliente()'>
        <h2 class='form__title form__title--registro mb-5'>Registrar Cliente</h2>
        <v-alert class="form__alert form__alert--registro" v-model="error" type="error" dense dismissible>{{errorMessage}}</v-alert>
        <div class="form__fields form__fields1--registro">
          <v-text-field label="Nombre del cliente" type="text" :rules="fieldRules"  v-model="nombre" outlined  required></v-text-field>
          <v-text-field label="Documento del cliente" type="text" :rules="fieldRules"  v-model="cedula" outlined  required></v-text-field>
          <v-text-field label="Email del cliente" type="email" :rules="fieldRules"  v-model="email" outlined  required></v-text-field>
        </div>
        <div class="form__fields form__fields2--registro">
          <v-text-field label="Apellido del cliente" type="text" :rules="fieldRules"  v-model="apellido" outlined  required></v-text-field>
          <v-text-field label="Telefono del cliente" type="tel" :rules="fieldRules"  v-model="telefono" outlined  required></v-text-field>
          <v-text-field label="Contraseña" type="password" :rules="fieldRules"  v-model="password" outlined  required></v-text-field>
        </div>
        <v-btn class="form__button form__button--registro" block elevation="2">Registrar</v-btn>
      </v-form>
    </v-card>
  </div>
</template>

<script>
  export default {
    name: 'Registro',

    computed:{
      
    },

    data(){
      return{
        user: '',
        password: '',
        rol: 'admin',
        error: false,
        errorMessage:'',
        fieldRules: [v => !!v || 'Campo requerido']
      }
    }
  }
</script>