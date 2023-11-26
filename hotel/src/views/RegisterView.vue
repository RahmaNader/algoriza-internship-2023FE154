<template>
    <div class="registration">
      <RegistrationForm />
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
import RegistrationForm from '@/components/RegistrationForm.vue';
  
  export default {
    name: 'RegisterView',
    components: {
        RegistrationForm
}
  }
  </script>
  