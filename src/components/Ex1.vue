<script>
    const fruits = ['apple', 'orange', 'peach']
    export default { 
        data() {
            return {
                message: "Choose your favorite fruit:",
                fruit1: fruits[0],
                fruit2: fruits[1],
                fruit3: fruits[2]
            }
        }
    }
</script>

<template>
    <div id="app">
        {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit">
    </div>
</template>

<style scoped>
</style>
