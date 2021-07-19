<template>
  <div class="posts">
    <ul class="c-posts">
      <li class="c-posts__item">
        <div class="posts__img">
          <img :src="avatar" alt="beb">
        </div>
        <span class="posts__username">{{ username }}</span>
      </li>
    </ul>
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
