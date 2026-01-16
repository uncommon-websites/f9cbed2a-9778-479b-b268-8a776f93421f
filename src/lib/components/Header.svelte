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
                d="M14.9099 3.21018C16.161 4.46126 14.6059 8.04474 11.4365 11.2141C8.26715 14.3835 4.68364 15.9386 3.43256 14.6876C2.18149 13.4365 3.73659 9.85299 6.90598 6.68359C10.0754 3.51421 13.6588 1.95911 14.9099 3.21018Z"
                fill="currentColor"
              />
              <path
                opacity="0.5"
                d="M17.6289 5.92841C18.88 7.1795 17.3249 10.763 14.1555 13.9324C10.9861 17.1018 7.40263 18.6569 6.15156 17.4058C4.90048 16.1547 6.45558 12.5712 9.62496 9.40184C12.7944 6.23244 16.3778 4.67735 17.6289 5.92841Z"
                fill="currentColor"
              />
              <path
                opacity="0.3"
                d="M20.3471 8.64697C21.5982 9.89806 20.043 13.4815 16.8737 16.6509C13.7043 19.8204 10.1208 21.3754 8.8697 20.1244C7.61861 18.8733 9.17373 15.2898 12.3431 12.1204C15.5125 8.951 19.096 7.39592 20.3471 8.64697Z"
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
