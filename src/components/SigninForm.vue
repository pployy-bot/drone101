<template>
  <div class="login-container">
    <div class="logo-container">
      <div class="circle-1"></div>
      <div class="circle-2"></div>
      <h1 class="logo">Prototype</h1>
    </div>

    <form class="login-form">
      <input type="email" placeholder="Email" v-model="email">
      <input type="password" placeholder="Password" v-model="password">
      <button type="submit"
 class="sign-in-button">Sign In →</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: '',
      password: '',
    };
  },
  methods: {
    handleSubmit(event) {
      event.preventDefault();
      console.log('Email:', this.email);
      console.log('Password:', this.password);
    },
  },
};
</script>

<style>
.login-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height:80vh;
}

.logo-container {
  display: flex;
  align-items: center;
  margin-bottom:
 0px;
}

.circle-1 {
  width: 80px;
  height: 80px;
  background-color: #FFC107;
  border-radius: 50%;
}

.circle-2 {
  width: 60px;
  height: 60px;
  background-color: #F44336;
  border-radius: 50%;
}

.logo {
  font-size: 80px;
  font-weight: bold;
  color: #EC008C;
  margin-left: 10px;
}

.login-form {
  display: flex;
  flex-direction: column;
  width: 400px;
}

input {
  padding: 10px;
  margin-bottom: 10px;
  border: 1px solid #ccc;
  border-radius:
 5px;
}

.sign-in-button {
  background-color: #EC008C;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
</style>