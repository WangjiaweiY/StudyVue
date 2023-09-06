<template>
    <h3>将key属性添加到v-for中</h3>
    <p v-for="(item, index) of names" :key="index">{{ item }}</p>
</template>

<script>

export default {
    data() {
        return {
            names:["123","yyt","555"]
        }
    }
}

</script>