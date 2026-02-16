<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<header class="fixed top-0 left-0 right-0 z-50 bg-white/80 backdrop-blur-md border-b border-gray-100">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between items-center h-16">
      <!-- Logo and Nav -->
      <div class="flex items-center gap-8">
        <a href="/" class="flex items-center gap-2">
          <!-- LOGAID Logo -->
          <div class="w-8 h-8 text-primary-600">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
	<path
		opacity="0.7"
		d="M9.22279 15.2235C12.6595 15.2235 15.4456 12.4375 15.4456 9.00075C15.4456 5.56399 12.6595 2.77795 9.22279 2.77795C5.78604 2.77795 3 5.56399 3 9.00075C3 12.4375 5.78604 15.2235 9.22279 15.2235Z"
		fill="currentColor"
	/>
	<path
		opacity="0.7"
		d="M14.5566 20.5574C17.9933 20.5574 20.7794 17.7713 20.7794 14.3346C20.7794 10.8978 17.9933 8.11179 14.5566 8.11179C11.1198 8.11179 8.3338 10.8978 8.3338 14.3346C8.3338 17.7713 11.1198 20.5574 14.5566 20.5574Z"
		fill="currentColor"
	/>
</svg>
          </div>
          <span class="font-bold text-xl tracking-tight">LOGAID</span>
        </a>

        <nav class="hidden md:flex items-center gap-6">
          <a href="#product" class="text-sm font-medium text-gray-600 hover:text-gray-900">Produkt</a>
          <a href="#solutions" class="text-sm font-medium text-gray-600 hover:text-gray-900">Lösungen</a>
          <a href="#resources" class="text-sm font-medium text-gray-600 hover:text-gray-900">Ressourcen</a>
          <a href="#company" class="text-sm font-medium text-gray-600 hover:text-gray-900">Unternehmen</a>
        </nav>
      </div>

      <!-- Right Actions -->
      <div class="flex items-center gap-4">
        <a href="#login" class="text-sm font-medium text-gray-600 hover:text-gray-900 hidden sm:block">Log in</a>
        <Button variant="secondary" size="sm" class="!bg-black !text-white !rounded-full px-5">Book a demo</Button>
      </div>
    </div>
  </div>
</header>
