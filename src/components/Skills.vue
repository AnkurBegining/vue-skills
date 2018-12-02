<template>
    <div class="hello">
        <div class="holder">
            <ul>
                <li v-for="(data,index) in skills">
                    {{index}}. {{data.skill}}
                </li>
                <br>
            </ul>
            <p v-if="skills.length > 1"> Length of skill is more than 1</p>
            <p v-else>Length of skill is less than 1</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Skills',
        data(){
            return{
                skills: [
                    {
                        "skill" : "Python"
                    },
                    {
                        "skill" : "Vue.js"
                    },
                    {
                        "skill" : "Django"
                    },
                    {
                        "skill" : "Data Analytics"
                    },

                ]
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
