<template>
    <div>
        <v-data-table :headers="headers" :items="pqrs" :items-per-page="10" class="elevation-3 table table--users">
            <template v-slot:item.actions="{ item }">
                <v-btn elevation="2" small  @click="editItem(item)"><v-icon small>mdi-pencil</v-icon></v-btn>
                <v-btn elevation="2" small  @click="editItem(item)"><v-icon small>mdi-pencil</v-icon></v-btn>
                <v-btn elevation="2" small  @click="editItem(item)"><v-icon small>mdi-pencil</v-icon></v-btn>
                <v-btn elevation="2" small  @click="editItem(item)"><v-icon small>mdi-pencil</v-icon></v-btn>
            </template>
        </v-data-table>
        <p>{{dialog}}</p>
    </div>
</template>

<script>
  export default {
    data: () => ({
      dialog: 'dialogo',
      headers: [
        { text: 'Asunto', value: 'asunto' },
        { text: 'Tipo de solicitud', value: 'tipo' },
        { text: 'Fecha de creacion', value: 'fecha' },
        { text: 'Estado', value: 'estado' },
        { text: 'Actions', value: 'actions', sortable: false },
      ],
      users: []
    }),

    created () {
      this.initialize()
    },

    methods: {

      initialize () {
        this.pqrs = [
          {
            asunto: 'ddbdjubwedo dedirnbdif rnfdirnfdioer rbeiufcbrif',
            tipo: 'Peticion',
            fecha: '02/07/2020',
            estado: 'En proceso',
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
          {
            asunto: 'Jaimes',
            tipo: 'Jesus',
            fecha: 'correo@mail.com',
            estado: 3111111111,
          },
        ]
      },

      editItem (item) {
        this.dialog = item;
      },

    },
  }
</script>