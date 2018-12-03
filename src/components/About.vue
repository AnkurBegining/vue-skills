<template>
    <div class="about">
        <h1>This is about page and their name is {{ their_name }}</h1>
    </div>

</template>

<script>
    export default {
        name: "About",
        data() {
            return {
                their_name : this.$route.params.name
            }
        }
    }
</script>

<style scoped>

</style>
