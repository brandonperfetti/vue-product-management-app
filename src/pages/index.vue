<script setup lang="ts">
import { supabase } from '@/lib/supabaseClient'
;(async () => {
  const { data, error } = await supabase.from('projects').select()
  if (error) {
    console.error(error)
  }
  console.log('Projects: ', data)
})()
</script>

<template>
  <div>
    <h1>Home Page</h1>
    <RouterLink :to="{ name: '/projects/[id]', params: { id: 1 } }">Go to project 1</RouterLink>
  </div>
</template>
