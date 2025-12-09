<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="pt-32 pb-16 overflow-hidden">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="max-w-4xl mx-auto text-center mb-16">
      <h1 class="text-5xl md:text-6xl font-semibold tracking-tight text-gray-900 mb-6 leading-[1.1]">
        Activate customers and ensure secure transactions at scale
      </h1>
      <p class="text-xl text-gray-600 mb-10 max-w-2xl mx-auto leading-relaxed">
        Bird powers your fintech platform with compliant messaging, instant authentication, and lifecycle campaigns that build trust.
      </p>
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <Button variant="primary" size="lg" class="rounded-full px-8">Contact sales</Button>
        <Button variant="outline" size="lg" class="rounded-full px-8">Get started</Button>
      </div>
    </div>

    <!-- Logos Strip -->
    <div class="mb-12">
      <p class="text-xs font-semibold text-gray-500 uppercase tracking-wider mb-6 text-left sm:ml-4">Trusted by 5000+ companies<br>that depend on Bird</p>
      <div class="flex flex-wrap items-center justify-between gap-8 opacity-60 grayscale px-4">
        <!-- Pinterest -->
        <svg class="h-8" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.373 0 0 5.373 0 12c0 5.084 3.163 9.426 7.627 11.174-.105-.949-.2-2.405.042-3.441.218-.937 1.407-5.965 1.407-5.965s-.359-.719-.359-1.782c0-1.668.967-2.914 2.171-2.914 1.023 0 1.518.769 1.518 1.69 0 1.029-.655 2.568-.994 3.995-.283 1.194.599 2.169 1.777 2.169 2.133 0 3.772-2.249 3.772-5.495 0-2.873-2.064-4.882-5.012-4.882-3.65 0-5.789 2.738-5.789 5.57 0 1.103.425 2.286.956 2.929.105.128.12.24.089.373-.098.407-.318 1.289-.361 1.47-.057.237-.188.287-.433.173-1.616-.752-2.626-3.116-2.626-5.014 0-4.08 2.969-7.828 8.568-7.828 4.498 0 7.994 3.207 7.994 7.55 0 4.505-2.839 8.131-6.779 8.131-1.323 0-2.566-.688-2.992-1.501l-.814 3.102c-.297 1.135-1.1 2.56-1.639 3.429 1.23.366 2.531.565 3.88.565 6.627 0 12-5.373 12-12S18.627 0 12 0z"/></svg>
        <!-- Uber -->
        <svg class="h-6" viewBox="0 0 24 24" fill="currentColor"><path d="M12 24C5.373 24 0 18.627 0 12S5.373 0 12 0s12 5.373 12 12-5.373 12-12 12zm7.2-4.8c1.2-1.8 1.8-3.6 1.8-6s-.6-4.2-1.8-6c-1.2-1.8-3-2.4-5.4-2.4-2.4 0-4.2.6-5.4 2.4-1.2 1.8-1.8 3.6-1.8 6s.6 4.2 1.8 6c1.2 1.8 3 2.4 5.4 2.4 2.4 0 4.2-.6 5.4-2.4zM8.4 12c0-3.6 1.8-5.4 5.4-5.4 1.8 0 3 .6 3.6 1.8.6 1.2.6 2.4.6 3.6 0 3.6-1.8 5.4-5.4 5.4-1.8 0-3-.6-3.6-1.8-.6-1.2-.6-2.4-.6-3.6z"/></svg>
        <!-- Square -->
        <svg class="h-8" viewBox="0 0 24 24" fill="currentColor"><path d="M19.65 4.35h-15.3v15.3h15.3V4.35zM24 0v24H0V0h24zM6.9 6.9h10.2v10.2H6.9V6.9zm2.55 2.55v5.1h5.1v-5.1H9.45z"/></svg>
        <!-- Airwallex (Text fallback) -->
        <span class="text-2xl font-bold font-sans tracking-tighter">Airwallex</span>
        <!-- Adobe -->
        <svg class="h-8" viewBox="0 0 24 24" fill="currentColor"><path d="M15.1 2H24v20L15.1 2zM8.9 2H0v20L8.9 2zM12 9.4L17.6 22h-3.8l-1.6-4H8.1L12 9.4z"/></svg>
      </div>
    </div>

    <!-- Hero Image -->
    <div class="relative rounded-2xl overflow-hidden shadow-2xl bg-gray-100">
      <img 
        src="https://images.unsplash.com/photo-1556761175-5973dc0f32e7?ixlib=rb-4.0.3&auto=format&fit=crop&w=2000&q=80" 
        alt="Person using fintech app" 
        class="w-full h-[600px] object-cover object-center"
      />
      
      <!-- Floating UI Elements -->
      <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 flex flex-col gap-4">
        <!-- Notification 1 -->
        <div class="bg-white/90 backdrop-blur-sm p-4 rounded-xl shadow-lg flex items-center gap-4 animate-in fade-in slide-in-from-bottom-4 duration-700">
          <div class="w-10 h-10 bg-gray-900 rounded-full flex items-center justify-center text-white">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
          </div>
          <div>
            <div class="text-sm font-semibold text-gray-900">ATM withdrawal</div>
            <div class="text-xs text-gray-500">$100 from Main Street ATM</div>
          </div>
        </div>

        <!-- Notification 2 -->
        <div class="bg-white/90 backdrop-blur-sm p-4 rounded-xl shadow-lg flex items-center gap-4 ml-12 animate-in fade-in slide-in-from-bottom-4 duration-1000 delay-300">
          <div class="w-10 h-10 bg-gray-900 rounded-full flex items-center justify-center text-white">
             <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="12" y1="1" x2="12" y2="23"></line><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path></svg>
          </div>
          <div>
            <div class="text-sm font-semibold text-gray-900">Transaction received</div>
            <div class="text-xs text-gray-500">You received $45.00 from Paul</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
