<script setup>
import GroupCard from '@/components/GroupCard.vue'
import { ref } from 'vue'

const awesome = ref(false)
</script>

<template>
  <main>
    <div id="display">
      <div id="groupSidebar">
        <div id="groupsWrapper">
          <GroupCard>
            <template #groupname>Group 1</template>
            <li>User 1</li>
            <li>User 2</li>
          </GroupCard>
          <GroupCard>
            <template #groupname>Group 2</template>
            <li>User 1</li>
            <li>User 2</li>
            <li>User 3</li>
          </GroupCard>
          <GroupCard>
            <template #groupname>Group 3</template>
            <li>User 1</li>
            <li>User 2</li>
            <li>User 3</li>
            <li>User 4</li>
          </GroupCard>
          <GroupCard>
            <template #groupname>Group 4</template>
            <li>User 1</li>
          </GroupCard>
        </div>
        <a href="/">Return</a>
      </div>
    </div>
  </main>
</template>

<style scoped>
a {
  text-decoration: none;
  color: var(--color-text);
}

#display {
  height: 100vh;
}

#groupSidebar {
  display: flex;
  flex-direction: column;
  width: fit-content;
  height: 100%;
  border-right: 1px solid var(--color-border);
}

#groupSidebar > a {
  padding: .5rem 0;
  margin-top: auto;
  width: 100%;
  border-top: 1px solid var(--color-border);
  color: #4DB6AC;
  text-align: center;
  transition: 0.5s;
}

#groupSidebar > a:hover {
  background-color: #4DB6AC;
  color: var(--color-background);
  font-weight: bold;
}

#groupsWrapper {
  display: inline-block;
}
</style>
