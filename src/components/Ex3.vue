<script>
    export default { 

       // add code here
       data() {
            return  {
                selectedInput: 'username'
            }
       }

    }
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
    <select v-model="selectedInput">
        <option value='username' selected>Username login</option>
        <option value="email">Email login</option>
    </select>
    
    <div>
        <label>Username</label>
        <input v-if="selectedInput == 'username'" placeholder="Enter your username">
        <input v-else type="email" placeholder="Enter your email">
    </div>
</template>

