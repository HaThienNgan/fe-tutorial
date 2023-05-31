<template>
  <div class="container mx-auto">
    <div class="grid grid-cols-4 mt-10">
      <div class="col-span-2">
        <h1 class="font-medium text-5xl mb-4">Nuxt Docs</h1>
        <p class="font-normal text-lg pr-20">Nuxt is a free and open-source framework with an intuitive and extendable way to create type-safe, performant and production-grade full-stack web applications and websites with Vue.js.</p>
      </div>
      <div class="col-span-2"></div>
    </div>
    <div class="border rounded-md p-4 mt-10">
      <h4 class="font-medium text-lg mb-4">Getting Started</h4>
      <p class="text-slate-500">Start by learning Nuxt core features, from installation to deployment.</p>
      <button class="py-1 px-4 mt-4 mr-2 bg-black text-white rounded-md outline outline-blue-500">Get started</button>
      <button class="border py-1 px-4 rounded-md hover:bg-slate-100">Explpre Examples</button>
    </div>
    <div class="mb-6">
      <h1 class="font-medium text-5xl mb-4 mt-8">API</h1>
      <p class="font-normal text-lg pr-20">Every Nuxt component, composable and utility, in detail.</p>
      <div class="grid grid-cols-3 gap-8 mt-4 ">
        <LandingPageApiCard imgSrc="/images/composables-light.svg" title="Composables" content="From data fetching to error handling, get familiar with Nuxt built-in composables." />
        <LandingPageApiCard title="Components" content="Nuxt components, auto-imported and ready to use in your application." />
        <LandingPageApiCard title="Utils" content="Use utility functions to get fine-grained control over your app behavior." />
        <LandingPageApiCard title="Advanced" content="Learn about lifecycle hooks and Kit utilities in the advanced section.." />
        <LandingPageApiCard title="Commands" content="Meet Nuxi, Nuxt 3 command-line tool. The essential companion in your journey." />
        <LandingPageApiCard title="Configuration" content="Master the Nuxt config file to customize the framework behavior." />
      </div>
    </div>
  </div>
</template>

<script>

</script>
