<template>
    <div class="topline">
      <topline>
        <template #headline>
          <div class="header">
            <a class="logo">
              <icon name="gitogram" />
            </a>
            <div class="navigation">
              <div class="icon">
              <icon name="home" />
            </div>
              <div class="icon">
                <icon name="out" />
              </div>
            </div>
          </div>
        </template>
        <template #content>
          <ul class="stories">
            <li class="stories__item" v-for="story in stories" :key="story.id">
              <story-user-item :avatar="story.avatar" :username="story.username"/>
            </li>
          </ul>
        </template>
      </topline>
      <template>
        <posts />
      </template>
    </div>
</template>
<script>
import { topline } from '../../components/topline'
import { storyUserItem } from '../../components/storyUserItem'
import { icon } from '../../icons'
import { posts } from '../../components/posts'
import stories from './data.json'

export default {
  name: 'feeds',
  components: {
    topline,
    icon,
    storyUserItem,
    posts
  },
  data () {
    return {
      stories
    }
  }
}
</script>

<style src="./feeds.scss" lang="scss" scoped></style>
