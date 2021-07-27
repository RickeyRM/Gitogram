<template>
  <div class="container">
    <ul class="posts__inner">
      <li class="posts__item">
        <div class="posts__user">
          <div class="posts__img">
            <img :src="avatar" alt="beb">
          </div>
          <span class="posts__username">{{ username }}</span>
        </div>
        <div class="posts__repository">
          <slot name="repository"></slot>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'posts'
}
</script>
<style lang="scss" src="./posts.scss" scoped></style>
