<template>
    <div class="solicitud">
        <v-card elevation="3">
            <v-form class="pa-10 form form--solicitud">
                <h2 class='form__title form__title--solicitud'>Nueva solicitud PQRS</h2>
                <v-alert class="form__alert form__alert--solicitud" v-model="error" type="error" dense dismissible>{{errorMessage}}</v-alert>
                <v-text-field class="form__fields1--solicitud" label="Asunto" type="text" :rules="fieldRules"  v-model="asunto" outlined required></v-text-field>
                <v-select class="form__fields2--solicitud" :items="items" label="Tipo de solicitud" outlined></v-select>
                <v-textarea class="form__textareas--solicitud" auto-grow outlined label="Escriba su solicitud" required></v-textarea>
                <v-file-input  class="form__fields form__fields3--solicitud" v-model="files" label="Adjuintar archivos" chips multiple outlined></v-file-input>
                <v-btn class="form__button form__button--solicitud" block>Crear solicitud</v-btn>
            </v-form>
        </v-card>
    </div>
</template>

<script>
  export default {
    name: 'NewPQRS',

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