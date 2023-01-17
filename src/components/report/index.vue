<template>
  <div class="report">
    <div @click="reportClick">
      <img src="../../assets/images/report.svg" alt="like" />
    </div>
  </div>
</template>

<script lang="ts">
export default {
  data() {
    return {
    }
  },
  methods: {
    reportClick() {
      alert('report success!')
    }
  }
}
</script>
<style scoped>
.report {
  opacity: 0.3;
}
</style>
