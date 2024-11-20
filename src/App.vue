<template>
  <q-page>
    <SigninForm msg="Welcome to Your Quasar App" />
  </q-page>
</template>

<script>
import SigninForm from './components/SigninForm.vue';

export default {
  name: 'App',
  components: {
    SigninForm
  }
}
</script>