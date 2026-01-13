<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="pt-32 pb-16 overflow-hidden">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="max-w-4xl mx-auto text-center mb-16">
      <h1 class="text-5xl md:text-6xl font-semibold tracking-tight text-gray-900 mb-6 leading-[1.1]">
        Transform logistics email chaos into automated efficiency
      </h1>
      <p class="text-xl text-gray-600 mb-10 max-w-2xl mx-auto leading-relaxed">
        LOGAID uses AI to classify, draft, and route thousands of logistics emails instantly—saving your team hours every day.
      </p>
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <Button variant="primary" size="lg" class="rounded-full px-8">Book a demo</Button>
        <Button variant="outline" size="lg" class="rounded-full px-8">See how it works</Button>
      </div>
    </div>

    <!-- Logos Strip -->
    <div class="mb-12">
      <p class="text-xs font-semibold text-gray-500 uppercase tracking-wider mb-6 text-left sm:ml-4">Trusted by logistics providers<br>processing millions of emails</p>
      <div class="flex flex-wrap items-center justify-center gap-12 opacity-60 grayscale px-4">
        <!-- DHL -->
        <span class="text-3xl font-bold font-sans tracking-tight">DHL</span>
        <!-- Maersk -->
        <span class="text-2xl font-bold font-sans tracking-tighter">MAERSK</span>
        <!-- Kuehne+Nagel -->
        <span class="text-2xl font-bold font-sans tracking-tight">Kuehne+Nagel</span>
        <!-- DB Schenker -->
        <span class="text-2xl font-bold font-sans tracking-tight">DB SCHENKER</span>
        <!-- DSV -->
        <span class="text-2xl font-bold font-sans tracking-wider">DSV</span>
      </div>
    </div>

    <!-- Hero Image -->
    <div class="relative rounded-2xl overflow-hidden shadow-2xl bg-gray-100">
      <img 
        src="https://images.unsplash.com/photo-1586528116311-ad8dd3c8310d?ixlib=rb-4.0.3&auto=format&fit=crop&w=2000&q=80" 
        alt="Logistics operations center" 
        class="w-full h-[600px] object-cover object-center"
      />
      
      <!-- Floating UI Elements -->
      <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 flex flex-col gap-4">
        <!-- Notification 1 -->
        <div class="bg-white/90 backdrop-blur-sm p-4 rounded-xl shadow-lg flex items-center gap-4 animate-in fade-in slide-in-from-bottom-4 duration-700">
          <div class="w-10 h-10 bg-primary-600 rounded-full flex items-center justify-center text-white">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
          </div>
          <div>
            <div class="text-sm font-semibold text-gray-900">Quote Request Classified</div>
            <div class="text-xs text-gray-500">FCL Shanghai → Rotterdam</div>
          </div>
        </div>

        <!-- Notification 2 -->
        <div class="bg-white/90 backdrop-blur-sm p-4 rounded-xl shadow-lg flex items-center gap-4 ml-12 animate-in fade-in slide-in-from-bottom-4 duration-1000 delay-300">
          <div class="w-10 h-10 bg-green-600 rounded-full flex items-center justify-center text-white">
             <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"></polyline></svg>
          </div>
          <div>
            <div class="text-sm font-semibold text-gray-900">Draft Response Ready</div>
            <div class="text-xs text-gray-500">Review and send in 1 click</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
