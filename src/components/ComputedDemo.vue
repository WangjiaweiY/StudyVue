<template>
    <h3>{{ wangjiawei.name }}</h3>
    <p>{{ wangjiaweiContent }}</p>
</template>

<script>

    export default {
        data() {
            return {
                wangjiawei: {
                    name:"Fish",
                    content:["1","2","3"]
                }
            }
        },
        computed: {
            wangjiaweiContent() {
                return this.wangjiawei.content.length > 0 ? 'Yes' : 'No'
            }
        }
    }

</script>