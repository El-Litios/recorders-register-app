<template>
    <div>
        <br>
        <h5>Selecciona tus competencias</h5>
        <v-row class="gridButtons" >
            <v-btn-toggle multiple max="4">
                <v-col cols="12" md="12" class="ColTopBtns">
                    <v-btn value="1">
                        Gestion
                    </v-btn>
                    <v-btn value="2">
                        Trabajo en Equipo
                    </v-btn>
                    <v-btn value="3">
                        Docencia
                    </v-btn>
                    <v-btn value="4">
                        Creatividad
                    </v-btn>
                    <v-btn value="5">
                        Liderazgo
                    </v-btn>
                </v-col>
                <v-col cols="12" md="12" class="ColBopBtns">
                    <v-btn value="6">
                        Investigacion
                    </v-btn>
                    <v-btn value="7">
                        Comunicacion
                    </v-btn>
                    <v-btn value="8">
                        Agilidad
                    </v-btn>
                    <v-btn value="9">
                        Responsabilidad
                    </v-btn>
                    <v-btn value="10">
                        Compromiso
                    </v-btn>
                </v-col>
            </v-btn-toggle>
            
        </v-row>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    @import 'GridButtons.css';
</style>