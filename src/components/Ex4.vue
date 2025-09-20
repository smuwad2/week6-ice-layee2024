<script>
    export default { 
        data() {
            return {
                // Add code here
                id: 'demo1',
                isBlue: true

            }
        },
        methods: { 
   			// Add code here
            handleClick() {
                this.isBlue = !this.isBlue
            }
		}
    }
</script>

<template>
    <!-- Modify code here -->
    <div class="container">
        <div v-bind:id="id" class="m-2" v-bind:class="[isBlue ? 'blueBox' : 'redBox']">
            div ID : {{id}} 
        </div>
        
        <button type="button" 
        v-bind:class="[isBlue ? 'btn btn-secondary' : 'btn btn-danger']" 
        v-on:click="handleClick">Change Color</button>
    </div>

</template>

<style scoped>
    .redBox {
        background-color: red;
    }
    .blueBox {
        background-color: blue;
    }
    #demo1 {
        color: white;
    }
</style>
