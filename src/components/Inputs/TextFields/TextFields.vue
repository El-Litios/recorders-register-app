<template>
    <div>
        <h5>NOMBRE</h5>
        <v-text-field label="Ej: Carlos Perez" v-model="name" :rules="nameRules" required solo></v-text-field>
        <h5>CORREO</h5>
        <v-text-field solo v-model="email" :rules="emailRules" label="E-mail" required></v-text-field>
        <h5>TU PERFIL TI</h5>
    </div>
</template>

<script>
export default {
    data () {
        return{
            name: '',
            nameRules: [
                v => !!v || 'Debe ingresar su nombre',
            ],
            email: '',
            emailRules: [
                v => !!v || 'Debe ingresar su email',
                v => /.+@.+\..+/.test(v) || 'Debe ser un email valido',
            ],
        }
    }
}
</script>

<style scoped>
    @import 'TextFields.css';
</style>