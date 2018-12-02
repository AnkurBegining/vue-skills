<template>
    <div class="hello">
        <div class="holder">
            <ul>
                <li v-for="(data,index) in skills">
                    {{index}}. {{data.skill}}
                </li>
            </ul>
            <p v-if="skills.length > 1"> Length of skill is more than 1</p>
            <p v-else>Length of skill is less than 1</p>
        </div>
        <div v-bind:class="{ alert: showAlert, another_class: showClass }"></div>
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

                ],
                showAlert: true,
                showClass: true
            }
        }

    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style src="./skill-style.css" scoped>

</style>
