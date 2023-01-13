<script >


import axios from 'axios';

const API_URL =  "http://localhost/";



export default {
  
  methods: {

    getAllData() {
      
      axios.get(API_URL + "api.php")
           .then(res => {

            const data = res.data;

            console.log(data);
           });
    },
    
  },
  mounted() {
    
    this.getAllData();
  }
}

</script>

<template>
  
</template>

<style scoped>

</style>
