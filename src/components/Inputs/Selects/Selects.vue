<template>
    <v-row>
        <v-col cols="12" lg="6" md="6" sm="12" xs="12">
            <h5>PAIS DE RESIDENCIA</h5>
            <v-select label="Escoge tu Pais" :items="Paises" v-model="Pais" item-text="name" solo></v-select>
        </v-col>
        <v-col cols="12" lg="6" md="6" sm="12" xs="12">
            <h5>CIUDAD DE RESIDENCIA</h5>
            <v-select :items="ValidarCiudad" label="Escoge tu ciudad" v-model="Ciudad" :disabled="ValidarSelect" solo></v-select>
        </v-col>
    </v-row>
</template>

<script>
export default {
    data: () => ({
        Pais: null,
        Ciudad: null,
        Paises: [
            {
                name: 'Chile',
                ciudades: ['Santiago', 'Curicó', 'Valparaiso']
            },
            {
                name: 'Argentina',
                ciudades: ['La plata', 'Buenos Aires', 'Córdoba']
            },
            {
                name: 'Colombia',
                ciudades: ['Medellin', 'Bógota', 'Cali']
            }
        ]
    }),

    computed: {
        ValidarCiudad(){
            const locacion = this.Paises.find(l => l.name === this.Pais);

            return locacion ? locacion.ciudades : []
        },

        ValidarSelect(){
            return !this.Pais ? true : false;
        }
    }
}
</script>

<style scoped>
    @import 'Selects.css';
</style>