<template>
    <div class="register-form">
      <h1>Register</h1>
      <form @submit.prevent="register">
        <div class="form-group">
          <label for="email">Email address</label>
          <input type="email" id="email" v-model="registerForm.email" required>
        </div>
        <div class="form-group">
          <label for="password">Password</label>
          <input type="password" id="password" v-model="registerForm.password" required>
        </div>
        <div class="form-group">
          <label for="confirmPassword">Confirm password</label>
          <input type="password" id="confirmPassword" v-model="registerForm.confirmPassword" required>
        </div>
        <button type="submit">Submit</button>
      </form>
      <p>
        Already have an account? <router-link to="/login">Login</router-link>
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
      register() {
        if (this.registerForm.password !== this.registerForm.confirmPassword) {
          alert('Passwords do not match');
          return;
        }
  
        // Send registration data to your backend server
        /*
        axios.post('/api/register', this.registerForm)
          .then((response) => {
            console.log('Registration successful:', response.data);
            // Handle successful registration
          })
          .catch((error) => {
            console.error('Registration failed:', error);
            // Handle registration error
          });
          */
      }
    }
  }
  </script>
    
  <style scoped>
  .register-form {
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
    