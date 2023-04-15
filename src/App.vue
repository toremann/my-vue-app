<script setup>
import Register from './components/Register.vue';
import TopNavBar from './components/TopNavBar.vue'
import GetData from './components/GetData.vue'
</script>

<template>
  <TopNavBar />
  <section class="flex items-center justify-center h-screen">
    <div class="max-w-5xl mx-auto">
      <header class="relative pt-20 sm:pt-24 lg:pt-32">
        <h1
          class="text-slate-900 font-extrabold text-4xl sm:text-5xl lg:text-6xl tracking-tight text-center dark:text-white gradient-text">
          Get some data.
        </h1>
        <p class="mt-6 text-lg text-slate-600 text-center max-w-3xl mx-auto dark:text-slate-400">
          Create a <code class="font-mono font-medium pink">user</code>,
          create <code class="font-mono font-medium pink">api key</code>
          get <code class="font-mono font-medium pink">data</code> ...
        </p>
      </header>
    </div>
  </section>

  <section class="login">
    <Register />
  </section>
</template>
