<script>
export default {
  data() {
    return {
      email: '',
      password: '',
    }
  }
}
</script>

<template>
  <div class="login">
    <from>
        <h1>Log In</h1>
        <br><h3>Email</h3>
        <div></div>
        <input v-model="email"> {{ email }}
        <br><h3>Password</h3>
        <div></div>
        <input v-model="password"> {{ password }}
        <div></div>
        <br><input type="submit" value="ยืนยันผล">

    </from>
  </div>
    

</template>

<style scoped>
  .login{
    position: fixed;

    width: 400px;
    height: 400px;
    border-style: solid;
    border-color: black;
    text-align: center;
  }
</style>