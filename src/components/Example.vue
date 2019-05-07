<template>
    <section>
        <div>hello: {{ message }}</div>
    </section>
</template>

<script>
export default {
    data() {
        return{
            message: null
        }
    },
    created(){
        this.message = this.$store.getters.getMessage;
    }
}
</script>

<style lang="scss" scoped>
    $primarycolor: #333;
    div{
        color: $primarycolor;
    }
</style>
