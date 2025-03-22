<template>
    <a href=""><div class="card">
    <h3>
        <slot name="groupname"></slot>
    </h3>
    <div class="members">
      <b>Balance:</b>
      <p>
        $<slot name="balance"></slot>
      </p>
    </div>
  </div></a>
  
</template>

<style scoped>
a {
    text-decoration: none;
}

.card {
    padding: 1rem;
    width: 200px;
    border-bottom: 1px solid var(--color-border);
}

.members {
  /* margin-left: auto; */
  /* display: flex;
  flex-direction: column; */
  /* background-color: antiquewhite; */
}

h3 {
    color: var(--color-heading);
}

b {
  /* color: #4DB6AC; */
  width: 100%;
  font-size: 12px;
  text-align: center;
}

p {
  color: #4DB6AC;
  font-size: 18px;
  font-family: monospace;
}

ul {
    padding: 0;
    text-align: center;
    list-style: none;
    font-size: 11px;
}
</style>
