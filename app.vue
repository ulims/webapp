<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtWelcome />
  </div>
</template>
<script setup>
useHead({
  meta: [
    { 
      name: 'apple-itunes-app', 
      content: `app-id=com.example.customer, app-argument=https://trychow.vercel.app/restaurant/${restaurantId}`
    },
    {
      name: 'google-play-app',
      content: 'app-id=com.example.customer'
    }
  ],
  link: [
    {
      rel: 'alternate',
      href: `android-app://com.example.customer/https/trychow.vercel.app/restaurant/${restaurantId}`
    }
  ]
})
</script>