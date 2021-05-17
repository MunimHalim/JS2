<template>
    <div>
        <h1>This is the home page</h1>
        <img @click="turnIt" id="lamb" src="https://www.w3schools.com/js/pic_bulboff.gif">
    </div>
</template>

<script>
    // @ is an alias to /src

    export default {
        name: 'home',
        components: {},
        data() {
            return {
                name: "Islam",
            }
        },
        methods: {
            turnIt() {
                let lamb = document.getElementById('lamb');
                if (lamb.src == "https://www.w3schools.com/js/pic_bulboff.gif") {
                    lamb.src = "https://www.w3schools.com/js/pic_bulbon.gif"
                } else {
                    lamb.src = "https://www.w3schools.com/js/pic_bulboff.gif"
                }
            }
        },
    }

</script>
<style scoped>
    img {
        cursor: pointer;
    }
</style>
