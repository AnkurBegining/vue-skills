<template>
    <div>
        {{name}}
        {{ btnState === true ? "Button is disabled" : "Button is not disabled" }}
        <button v-on:click="changeName" v-bind:disabled="btnState">Change Me</button>
    </div>
</template>

<script>
    export default {
        name: 'Skills',
        data(){
            return{
                name : "Ankur",
                btnState : true
            }
        }

    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    h3 {
        margin: 40px 0 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
</style>
