<template>
    <div class="topline">
      <topline>
        <template #headline>
          <div class="header">
            <a class="icon">
              <icon name="gitogram" />
            </a>
            <div class="icon">
              <icon name="home" />
              <icon name="out" />
            </div>
          </div>
        </template>
        <template>
          <story-user-item avatar="https://picsum.photos/300/300" username="Jhon"/>
        </template>
      </topline>
    </div>
</template>
<script>
import { topline } from '../../components/topline'
import { storyUserItem } from '../../components/storyUserItem'
import { icon } from '../../icons'

export default {
  name: 'feeds',
  components: {
    topline,
    icon,
    storyUserItem
  }
}
</script>

<style lang="scss" scoped>
  .icon{
    width: 24px;
    color: #262626;

  }
  .header{
    display: flex;
    justify-content: space-between;
  }
</style>
