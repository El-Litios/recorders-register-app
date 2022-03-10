<template>
  <div class="AvatarImage">
      <div class="img-avatar" v-if="!preview">
          <v-img src="../../../assets/Avatar.jpg" width="350" height="350" position='center center'></v-img>
      </div>
      <div class="img-avatar" v-else>
          <v-img :src="preview" width="350" height="350"></v-img>
      </div>
      <input accept="image/*" @change="previewImage" class="foo" type="file">
  </div>
</template>

<script>
export default {
  data () {
    return {
      preview: null,
      image: null,
    }
  },

   methods: {
    previewImage: function(event) {
      var input = event.target;
      if (input.files) {
        var reader = new FileReader();
        reader.onload = (e) => {
          this.preview = e.target.result;
        }
        this.image=input.files[0];
        reader.readAsDataURL(input.files[0]);
      }
    },
  }
}
</script>

<style scoped>
  @import 'Avatar.css';
</style>