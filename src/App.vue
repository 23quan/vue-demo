<template>
  <div>
    <p>{{ msg }}</p>

    <p v-if="show">true显示文字</p>

    <div v-if="Math.random() > 1">随机数大于1</div>

    <div v-else>随机数小于1</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "vue展示",
      show: true,
      namelist: [
        { text: "斯内克" },
        { text: "爱丽丝" },
        { text: "张大炮" }
      ]
    }
  }
}
</script>
