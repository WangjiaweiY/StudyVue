<template>
    <h3>侦听器</h3>
    <p>{{ message }}</p>
    <button @click="updateHandle">修改数据</button>

</template>

<script>

export default {
    data() {
        return {
            message: "hello"
        }
    },
    methods: {
        updateHandle(){
            this.message = "world"
            console.log(this.message);
        }
    },
    watch: {
        message(newValue, oldValue) {
            
            console.log(newValue, oldValue);
        }
    }
}

</script>