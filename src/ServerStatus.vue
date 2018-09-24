<template>
   <div>
        <p>Server Status: {{ status }}</p>

        <hr>

        <button @click="changeStatus">Change Status</button>
    </div> 
</template>

<script>
export default {
  data: function() {
      return {
          status: 'Critical'
      }
  },

  methods: {
      changeStatus() {
         if (this.status == 'Critical') 
          this.status = 'Normal';
          else 
          {
              this.status = 'Critical'
          }
      }
  }
}
</script>

<style>

</style>
