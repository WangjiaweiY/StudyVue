<template>
    <h3>条件渲染</h3>
    <div v-if="flag">你能看见我么</div>
    <div v-else>那你还是看看</div>
    <div v-if="type === 'A'">A</div>
    <div v-else-if="type === 'B'">B</div>
    <div v-else-if="type === 'C'">C</div>
    <div v-else>Not A/B/C </div>
    <div v-show="flag">你能再次看见我么</div>
</template>

<script>
export default {
    data() {
        return {
            flag:true,
            type:"B"
        }
    }
}
</script>