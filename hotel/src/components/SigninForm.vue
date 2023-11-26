<template>
    <div class="signin-form">
      <h1>Sign in</h1>
      <form @submit.prevent="signin">
        <div class="form-group">
          <label for="email">Email address</label>
          <input type="email" id="email" v-model="registerForm.email" required>
        </div>
        <div class="form-group">
          <label for="password">Password</label>
          <input type="password" id="password" v-model="registerForm.password" required>
        </div>
        <button type="sign in">Submit</button>
      </form>
      <p>
        Don't have an account? <router-link to="/register">Register</router-link>
      </p>
    </div>
  </template>
    
  <script>
  export default {
    data() {
      return {
        registerForm: {
          username: '',
          email: '',
          password: '',
          confirmPassword: ''
        }
      }
    },
    methods: {
      
    }
  }
  </script>
    
  <style scoped>
  .signin-form {
    width: 500px;
    margin: 0 auto;
    padding: 20px;
    background-color: #fff;
    border: none;
  }
  
  .form-group {
    margin-bottom: 15px;
  }
  
  label {
    display: block;
    margin-bottom: 5px;
    color: #181818;
    font-style: normal;
    font-weight: normal;
    text-align: left;
    font-size: 20px;
  
  }
  
  input {
    width: 100%;
    padding: 5px;
    border: none;
    height: 44px;
    background-color: #F2F2F2;
    border-radius: 4px;
    font-size: 20px;
    line-height: 140%;
    letter-spacing: 0.02em;
  }
  
  button {
    width: 400px;
    height: 43px;
    background: #2F80ED;
    border-radius: 6px;
    border: none;
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 20px;
    /* identical to box height, or 133% */
    letter-spacing: 0.02em;
    color: #FFFFFF;
    cursor: pointer;
  
  }
  router-link {
    color: #2F80ED;
    cursor: pointer;
  }
  </style>
    