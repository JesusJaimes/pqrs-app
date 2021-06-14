<template>
    <div class='login'>
      <v-card elevation="3" class="pa-10">
        <v-form class="form form--login" @submit.prevent='submit()'>
          <div class="form__title  mb-5">
            <h2>Iniciar sesión</h2>
          </div>
          <v-alert v-model="error" type="error" dense dismissible>{{errorMessage}}</v-alert>
          <v-text-field v-model="user" label="User" type="text" :rules="fieldRules" outlined  required></v-text-field>
          <v-text-field v-model="password" label="Contraseña" type="password" :rules="fieldRules" outlined  required></v-text-field>
          <v-btn block elevation="2">Iniciar Sesión</v-btn>
        </v-form>
      </v-card>
    </div>
</template>

<script>
  export default {
    name: 'Login',

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