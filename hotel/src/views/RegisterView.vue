<template>
    <div class="home">
      <RegistrationForm />
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
import RegistrationForm from '@/components/RegistrationForm.vue';
  
  export default {
    name: 'HomeView',
    components: {
    RegistrationForm
}
  }
  </script>
  