<template>
    <p :class="{ 'active':isActive,'text-danger':hasError}">Class样式绑定1</p>
    <p :class="classObject">Class样式绑定2</p>
    <p :class="[arrActive,arrHasError]">Class样式绑定3</p>
    <p :class="[isActive ? 'active' : '']">Class样式绑定4</p>

</template>

<script>

    export default {
        data() {
            return {
                isActive:true,
                hasError:false,
                classObject:{
                    'active':true,
                    'text-danger':true
                },
                arrActive: "active",
                arrHasError: "text-danger"
            }
        }
    }

</script>

<style>

.active {
    
    font-size:30px;
}

.text-danger {
    color:red;
}

</style>