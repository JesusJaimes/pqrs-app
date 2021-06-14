<template>
    <div class="pqrs-info">
        <v-card elevation="3" class="mt-8 mb-6 pqrs-info--card">
            <v-card-title>Informacion de la solicitud</v-card-title>
            <v-card-subtitle><v-chip  color="primary" label>En proceso</v-chip></v-card-subtitle>
            
            <v-card-text>
                <v-divider></v-divider><br>
                <div>Asunto</div>
                <p class="text--primary font-weight-bold">
                    wcwedcwecwcwe
                </p>

                <div>Descripsión</div>
                <p class="text--primary">
                    wcwedcwecwcwecwcwecwcwecewcwcwecqwecwcewedcwecwecwecwecwecwcwqecwewcewcewcewcewcewcewcewcewcewcewcewceqeqeeeeeeeeeeq
                </p>

                <div>Archivos adjuntos</div>
                <v-chip class="ma-2" >Primary</v-chip>
                <v-chip class="ma-2" >Primarybbnkjjk</v-chip>
                <v-chip class="ma-2">Primary</v-chip>
                <v-chip class="ma-2" >Primacdscdscrybbnkjjk</v-chip>
                <v-chip class="ma-2" >Primarybbnkjjk</v-chip>
                <v-chip class="ma-2" >Primarybbnkjjk</v-chip>

                <v-divider class="mb-5"></v-divider>

                <v-card-title class="text--primary">Comentarios</v-card-title>

                <v-card class="mx-auto mb-4" outlined>
                    <v-card-text class="">
                        <div class="font-weight-bold text--primary">Persona</div>
                        <div class="text--primary">"Turns out semicolon-less style is easier and safer in TS because most gotcha edge cases are type invalid as well."</div>
                    </v-card-text>
                </v-card>
                
                <v-card class="mx-auto mb-4" color="grey" outlined>
                    <v-card-text class="text-right">
                        <div class="text--primary">"Turns out semicolon-less style is easier and safer in TS because most gotcha edge cases are type invalid as well."</div>
                    </v-card-text>
                </v-card>

                <v-form class="form text-right">
                    <v-textarea auto-grow rows="3" outlined label="Escribir un comentario" ></v-textarea>
                    <v-btn>Agregar comentario</v-btn>
                </v-form>
            </v-card-text>
        </v-card>
    </div>
</template>