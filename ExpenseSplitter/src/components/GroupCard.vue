<template>
    <a href=""><div class="card">
    <h3>
        <slot name="groupname"></slot>
    </h3>
    <div class="members">
      <ul>
        <!-- Change to prop and v-for later -->
        <slot></slot>
      </ul>
    </div>
  </div></a>
  
</template>

<style scoped>
a {
    text-decoration: none;
}

.card {
    padding: 1rem;
    border-bottom: 1px solid var(--color-border);
}

h3 {
    color: #4DB6AC;
    /* font-weight: bold; */
    /* font-size: 28px; */
}

ul {
    padding: 0;
    text-align: center;
    list-style: none;
    font-size: 11px;
}
</style>
