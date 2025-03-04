<script setup>
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <!-- <TheWelcome /> -->
    <div id="title">
      <h1>Expense Splitter</h1>
      <h3>Split expenses with friends easily.</h3>
      <div id="titleButton">
        <a href="/splitter">Open Splitter</a>
      </div>
    </div>
    <section>
      <!-- <p>
        <span></span>Effortlessly split and send bills to your friends with just a few taps.
        Have a recurring bill? 
        Set it up once, and we'll handle the rest—automatically tracking expenses and sending friendly reminders, so you never miss a payment.
      </p> -->
      <ul>
        <li><span>Easily split and send bills</span> to your friends with just a few taps.</li>
        <li><span>Set up recurring expenses</span> and let the app handle the rest.</li>
        <li><span>Automatic reminders</span> ensure everyone stays on top of their payments.</li>
        <li><span>Track shared expenses effortlessly</span> with a clear and organized overview.</li>
      </ul>
    </section>
  </main>
</template>

<style scoped>
h1 {
  color: #4DB6AC;
}

#title {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: white;
}

#titleButton {
  display: flex;
  margin-bottom: 4rem;
}

#titleButton a {
  margin-top: 2rem;
  padding: .5rem .75rem .5rem .75rem;
  background-color: var(--color-background);
  text-decoration: none;
  font-weight: bold;
  color: white;
  transition: 0.5s;
  border: 3px solid white;
  border-radius: 5px;
}

#titleButton a:hover {
  color: #4DB6AC;
  border-color: #4DB6AC;
}

section {
  /* margin: 2rem; */
  display: flex;
  justify-content: center;
  align-items: center;
}

ul {
  padding: 0 3rem 0 3rem;
}

li {
  margin-bottom: 1rem;
}

span {
  color: #4DB6AC;
  font-weight: bold;
}
</style>
