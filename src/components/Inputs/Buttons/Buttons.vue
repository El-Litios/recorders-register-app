<template>
  <v-btn-toggle tile multiple class="Buttons">
            <v-col cols="12" lg="12">
                <v-btn id="btn1" value="1">
                UX
                </v-btn>
                <v-btn id="btn2" value="2">
                UI
                </v-btn>
                <v-btn id="btn3" value="3">
                FULL STACK
                </v-btn>
            </v-col>
            <v-col cols="12" lg="12">
                <v-btn id="btn4" value="4">
                FRONT END
                </v-btn>
                <v-btn id="btn5" value="5">
                BACK END
                </v-btn>
            </v-col> 
    </v-btn-toggle>
</template>

<script>
export default {

}
</script>

<style scoped >
    @import 'Buttons.css';
</style>