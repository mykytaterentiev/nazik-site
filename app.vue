<template>
  <div class="container">
    <div class="verification">
      <div class="icon">
        <span>18+</span>
      </div>
      <h1>Age Verification</h1>
      <p>Are you at least 18 years old?</p>
      <button @click="confirmAge">Yes</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    confirmAge() {
      // Redirect to the desired page or handle logic
      this.$router.push('/home'); // Replace '/home' with your target route
    },
  },
};
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #f9f9f9;
}

.verification {
  text-align: center;
  padding: 2rem;
  background: white;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.icon {
  width: 100px;
  height: 100px;
  margin: 0 auto 1rem;
  border-radius: 50%;
  background: red;
  color: white;
  font-size: 2rem;
  font-weight: bold;
  display: flex;
  justify-content: center;
  align-items: center;
}

h1 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
}

p {
  margin-bottom: 1.5rem;
  color: #666;
}

button {
  padding: 0.75rem 1.5rem;
  border: none;
  background: #007bff;
  color: white;
  font-size: 1rem;
  border-radius: 5px;
  cursor: pointer;
  transition: background 0.3s;
}

button:hover {
  background: #0056b3;
}
</style>
