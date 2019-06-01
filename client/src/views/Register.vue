<template>
  <div class="home">
    <h1>Welcome to Your Register Page</h1>
    <input
      type="email"
      name="email"
      v-model="email"
      placeholder="email" 
    />
    <input
      type="password"
      name="password"
      v-model="password"
      placeholder="password"
    />
    <br />
    <button>Register</button>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  data() {
    return {
      email: "abc",
      password: "123"
    };
  },
  watch: {
    email(value) {
      console.log("email has changed", value)
    }
  }
};
</script>
