<section class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="mb-12">
      <div class="text-xs font-semibold text-gray-500 uppercase tracking-wider mb-4">Integrations</div>
      <h2 class="text-3xl font-semibold text-gray-900 mb-4">
        Bring all of your ecommerce apps together
      </h2>
      <p class="text-gray-500">Connect all your existing data and ecommerce tools in one place.</p>
      <a href="#" class="text-sm font-medium text-primary-600 hover:text-primary-700 flex items-center gap-1 mt-4">
        View all integrations 
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"></path><path d="m12 5 7 7-7 7"></path></svg>
      </a>
    </div>

    <div class="flex flex-wrap gap-4">
      {#each Array(10) as _, i}
        <div class="w-16 h-16 bg-gray-50 rounded-xl flex items-center justify-center grayscale opacity-80 hover:grayscale-0 hover:opacity-100 transition-all duration-300">
           <!-- Placeholder for app icons -->
           <div class="w-8 h-8 rounded bg-gray-300"></div>
        </div>
      {/each}
    </div>
  </div>
</section>
