<template>
  <div class="story__item">
    <button class="c-story-user-item">
    <div class="avatar">
      <img :src="avatar" class="avatar__img" alt="user">
    </div>
    <div class="username">
      {{ username }}
    </div>
  </button>
  </div>
</template>
<script>
export default {
  props: {
    avatar: {
      type: String,
      required: true
    },
    username: {
      type: String,
      required: true
    }
  }
}
</script>

<style src="./storyUserItem.scss" lang="scss" scoped>

</style>
