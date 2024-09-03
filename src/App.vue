<!--Top of document-->
<script lang="ts">

  export default {
    data() {
      return{
        name: 'Kevin Chang',
        status: false,
        tasks: ['Task One', 'Task Two', 'Task Three']
      };
    },
  };

</script>

<!--- ~~~~~~~~~~~ HTML under here -~~~~~~~~~~ -->

<template>
  <h1>{{ name }}</h1>
  <p v-if="status">Member is active</p>
  <p v-else><em>Inactive member</em></p>

  <br> <br> 
  <h3>Tasks:</h3>
  <ul>
    <li style="margin: 0 0 -10px 15px" v-for="task in tasks" :key="task">{{ task }}</li>
  </ul>

</template>


<!--- ~~~~~~~~~~~ CSS under here -~~~~~~~~~~ -->

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300..900;1,300..900&display=swap');
  
  * {
    font-family: "Rubik", sans-serif;
    margin: 0;
    padding: 5px;
    box-sizing: border-box;
  }
  

  .container {
    max-width: 1100px;
    margin: 0 auto;
  }

</style>
