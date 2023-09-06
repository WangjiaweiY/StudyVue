<template>
  <div :class="msg">测试</div>
  <button :disabled="isButton">Button</button>
  <div v-bind="OBJ">nihao</div>
</template>

<script>
export default {
  data() {
    return {
      msg:"active",
      isButton:false,
      OBJ: {
        class:"xclass",
        id:"xId"
      }
    }
  }
}
</script>

