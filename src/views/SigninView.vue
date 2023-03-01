<template>
<div class="Fsignup"></div><header>Sign Up</header>
  <br><form>

  
  Name <input type="text" v-model="stuName" name="" id="" maxlength="100">
  <br><br>
  
  Phone Number <input type="text" name="" id="">
    <br><br>


  Email <input type="text" name="" id="">
    <br><br>
  Password <input type="text" name="" id="">



<br><br>

  
  
  <br><input type="submit" value="Sign Up">
  {{ stuID }} {{ stuName }}
  </form>
  </template>
  
  <script setup >
  import {ref} from "vue";
  
  const stuID=ref("");
  const stuName=ref("");
  </script>
  
  <style scoped>
  
  </style>