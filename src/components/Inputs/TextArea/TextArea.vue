<template>
    <v-col cols="12" class="TxtArea">
      <h5>Escribe una reseña de tu vida profesional</h5>
      <v-textarea counter :rules="rules" v-model="value" :no-resize=true></v-textarea>
    </v-col>
</template>

<script>
export default {
    data: () => ({
      rules: [v => v.length <= 200 || 'Maximo 200 caracteres'],
      value: '',
    })
}
</script>

<style scoped>
    @import 'TextArea.css';
</style>