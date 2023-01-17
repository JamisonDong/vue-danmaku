<template>
  <div class="like">
    <div @click="likeClick">
      <img src="../../assets/images/liked.svg" alt="" v-if="flag">
      <img src="../../assets/images/like.svg" alt="" v-else>
    </div>
    <div>{{ likes }}</div>
  </div>
</template>

<script lang="ts">
export default {
  props: ['like'],
  
  data() {
    return {
      likes: this.like,
      flag: false,
    }
  },
  methods: {
    likeClick() {
      this.likes++;
      this.flag = true;
      //TODO: 异步更新点赞数量
    },
  }
}
</script>
<style scoped>
.like{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 60px;
}

</style>