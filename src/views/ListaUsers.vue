<template>
    <div>
        <v-data-table :headers="headers" :items="users" :items-per-page="10" class="elevation-3 table table--users">
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
        { text: 'Apellido', value: 'apellido' },
        { text: 'Nombre', value: 'nombre' },
        { text: 'E-mail', value: 'email' },
        { text: 'Telefono', value: 'tel' },
        { text: 'Actions', value: 'actions', sortable: false },
      ],
      users: []
    }),

    created () {
      this.initialize()
    },

    methods: {

      initialize () {
        this.users = [
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
          {
            apellido: 'Jaimes',
            nombre: 'Jesus',
            email: 'correo@mail.com',
            tel: 3111111111,
          },
        ]
      },

      editItem (item) {
        this.dialog = item;
      },

    },
  }
</script>