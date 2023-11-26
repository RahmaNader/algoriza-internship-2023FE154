<template>
    <div class="signin">
      <SigninForm />
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
import SigninForm from '@/components/SigninForm.vue';
  
  export default {
    name: 'SigninView',
    components: {
    SigninForm
}
  }
  </script>
  