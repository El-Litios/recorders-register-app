<template>
  <div>
    <v-container>
      <v-form>
        <v-row>
          <v-col cols="12" xs="12" sm="12" md="6">
            <TextFields/>
            <Buttons />
          </v-col>
          <v-col cols="12" xs="12" sm="12" md="6">
            <Avatar />
          </v-col>
        </v-row>
        <Selects />
        <v-row>
          <TextArea />
          <Tags />
        </v-row>
        <GridFields />
        <br>
        <div class="text-center">
          <v-btn id="Send">
          ENVIAR SOLICITUD
          </v-btn>
        </div>
      </v-form>
    </v-container>    
  </div>
</template>

<script>
import TextFields from '@/components/Inputs/TextFields/TextFields.vue';
import Buttons from '@/components/Inputs/Buttons/Buttons.vue';
import Selects from '@/components/Inputs/Selects/Selects.vue';
import TextArea from '@/components/Inputs/TextArea/TextArea.vue';
import Tags from '@/components/Inputs/Tags/Tags.vue';
import GridButtons from '@/components/Inputs/GridButtons/GridButtons.vue';
import GridFields from '../components/Inputs/GridFields/GridFields.vue';
import Avatar from '../components/Inputs/Avatar/Avatar.vue';

export default {
    components: {
        TextFields, Buttons, Selects, TextArea, Tags, GridButtons, GridFields,
        Avatar
    }
}
</script>

<style scoped>
  @import url('Home.css');
</style>