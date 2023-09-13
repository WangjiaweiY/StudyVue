<template>
    <h3>数组变化侦听</h3>
    <button @click="addListHandle">添加数据</button>
    <ul>
        <li v-for="(item,index) of names" :key="index">{{ item }}</li>
    </ul>
</template>

<script>

    export default {
        data() {
            return {
                names:["iwen","ime","frank","gaway"]
            }
        },
        methods: {
            addListHandle() {
                this.names.reverse()
                this.names = this.names.concat(["io"])
            }
        }
    }

</script>