<template>
    <h3>列表渲染</h3>
    <p v-for="item of names">{{ item }}</p>
    <p v-for="(item,index) of names">{{ item }}-{{ index }}</p>
    <div v-for="item in result">
        <p>{{ item.id }}</p>
        <p>{{ item.name }}</p>
    </div>
    <div>
        <p v-for="(value,key,index) of userInfo">{{ value }}-{{ key }}-{{ index }}</p>
    </div>
</template>

<script>

export default {
    data() {
        return {
            names:["王嘉炜","nihao","hahaha"],
            result: [{
                    "id":"2021117300",
                    "name":"Gaway"
                },
                {
                    "id":"18009130234",
                    "name":"fish"
                }
            ],
            userInfo:{
                name:"GAWAY",
                sno:"123"
            }
        }
    }
}
</script>