<template>
  <div class="text-tag">
    <v-icon v-if="icon" small class="mr-1">
      {{ "mdi-" + icon }}
    </v-icon>
    <span>{{ text }}</span>
  </div>
</template>

<script>
  export default {
    props: {
      icon: {
        type: String,
        default: "",
      },
      text: {
        type: String,
        default: "",
      },
    },

    computed: {
      tagHide() {
        return false;
      },
    },
  };
</script>

<style lang="scss" scoped>
  .text-tag {
    display: flex;
    align-items: center;
  }
</style>
