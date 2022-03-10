<template>
  <v-col cols="12">
    <h5>Nombra aquellas herramientas que dominas</h5>
    <vue-tags-input
      v-model="tag"
      :tags="tags"
      :autocomplete-items="filteredItems"
      :add-only-from-autocomplete="true"
      placeholder=""
      @tags-changed="newTags => tags = newTags"
    />
  </v-col>
</template>

<script>
import VueTagsInput from '@johmun/vue-tags-input';

export default {
    components: {VueTagsInput},
    data: () => ({
      tag: '',
      tags: [],
      autocompleteItems: [{
        text: 'FIGMA',
      }, {
        text: 'VUEJS',
      }, {
        text: 'JAVA',
      }, {
        text: 'HTML5',
      }, {
        text: 'CSS3',
      },{
        text: 'mySQL',
      },{
        text: 'MongoDB',
      },{
        text: 'REACTJS',
      },{
        text: 'ANGULAR',
      },{
        text: 'Spring',
      },{
        text: 'SpringBoot',
      },{
        text: 'AdobeXd',
      },{
        text: 'AAAAAAAAAdobeXd',
      }],
    }),

    computed: {
        filteredItems() {
            return this.autocompleteItems.filter(i => {
            return i.text.toLowerCase().indexOf(this.tag.toLowerCase()) !== -1;
        });
        },
    }
}
</script>

<style scoped>
    @import 'Tags.css';
</style>