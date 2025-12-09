<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<header class="fixed top-0 left-0 right-0 z-50 bg-white/80 backdrop-blur-md border-b border-gray-100">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between items-center h-16">
      <!-- Logo and Nav -->
      <div class="flex items-center gap-8">
        <a href="/" class="flex items-center gap-2">
          <!-- Bird Logo Placeholder -->
          <div class="w-8 h-8 bg-primary-600 rounded-lg flex items-center justify-center text-white">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M22 4s-.7 2.1-2 3.4c1.6 10-9.4 17.3-18 11.6 2.2.1 4.4-.6 6-2C3 15.5.5 9.6 3 5c2.2 2.6 5.6 4.1 9 4-.9-4.2 4-6.6 7-3.8 1.1 0 3-1.2 3-1.2z"></path>
            </svg>
          </div>
          <span class="font-bold text-xl tracking-tight hidden">Bird</span> <!-- Text hidden in screenshot, just logo? Actually screenshot shows just logo or maybe logo+text. Let's assume just logo or logo+text. Screenshot top left is small. Looks like logo + "Bird" text but text is small. -->
        </a>

        <nav class="hidden md:flex items-center gap-6">
          <a href="#product" class="text-sm font-medium text-gray-600 hover:text-gray-900">Product</a>
          <a href="#solutions" class="text-sm font-medium text-gray-600 hover:text-gray-900">Solutions</a>
          <a href="#resources" class="text-sm font-medium text-gray-600 hover:text-gray-900">Resources</a>
          <a href="#company" class="text-sm font-medium text-gray-600 hover:text-gray-900">Company</a>
        </nav>
      </div>

      <!-- Right Actions -->
      <div class="flex items-center gap-4">
        <a href="#login" class="text-sm font-medium text-gray-600 hover:text-gray-900 hidden sm:block">Log in</a>
        <Button variant="secondary" size="sm" class="!bg-black !text-white !rounded-full px-5">Contact sales</Button>
      </div>
    </div>
  </div>
</header>
