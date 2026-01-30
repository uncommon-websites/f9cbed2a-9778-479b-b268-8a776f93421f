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
                d="M10.8332 3.21558C11.4167 2.63208 12.3627 2.63208 12.9462 3.21558L15.0592 5.3286C15.6427 5.91211 15.6427 6.85811 15.0592 7.44163L12.9462 9.55462C12.3627 10.1381 11.4167 10.1381 10.8332 9.55462L8.72017 7.44163C8.13669 6.85811 8.13669 5.91211 8.72017 5.3286L10.8332 3.21558Z"
                fill="currentColor"
              />
              <path
                d="M16.1157 8.49812C16.6992 7.91465 17.6452 7.91465 18.2288 8.49812L20.3418 10.6112C20.9253 11.1946 20.9253 12.1407 20.3418 12.7242L18.2288 14.8372C17.6452 15.4207 16.6992 15.4207 16.1157 14.8372L14.0027 12.7242C13.4192 12.1407 13.4192 11.1946 14.0027 10.6112L16.1157 8.49812Z"
                fill="currentColor"
              />
              <path
                d="M5.55064 8.49812C6.13414 7.91465 7.08017 7.91465 7.66367 8.49812L9.77667 10.6112C10.3602 11.1946 10.3602 12.1407 9.77667 12.7242L7.66367 14.8372C7.08017 15.4207 6.13414 15.4207 5.55064 14.8372L3.43762 12.7242C2.85413 12.1407 2.85413 11.1946 3.43762 10.6112L5.55064 8.49812Z"
                fill="currentColor"
              />
              <path
                d="M10.8332 13.7807C11.4167 13.1972 12.3627 13.1972 12.9462 13.7807L15.0592 15.8937C15.6427 16.4772 15.6427 17.4232 15.0592 18.0067L12.9462 20.1197C12.3627 20.7032 11.4167 20.7032 10.8332 20.1197L8.72017 18.0067C8.13669 17.4232 8.13669 16.4772 8.72017 15.8937L10.8332 13.7807Z"
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
