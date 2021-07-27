<template>
    <button class="stories__user-item">
      <div class="stories__avatar">
        <img :src="avatar" class="stories__avatar-img" alt="user">
      </div>
      <div class="username">
        {{ username }}
      </div>
    </button>
</template>
<script>
export default {
  name: 'storyUserItem',
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
