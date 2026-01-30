<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<footer class="bg-white pt-24 pb-12 border-t border-gray-100">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-8 mb-16">
      <!-- Column 1 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Produkt</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Übersicht</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">E-Mail-Klassifizierung</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">KI-Entwürfe</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Integrationen</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Analytics</a>
      </div>

      <!-- Column 2 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Lösungen</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Spediteure</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">3PL-Anbieter</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Zollmakler</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Frachtführer</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Lagerhaltung</a>
      </div>

      <!-- Column 3 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Ressourcen</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Blog</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Fallstudien</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Dokumentation</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">API-Referenz</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Hilfecenter</a>
      </div>

      <!-- Column 4 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Unternehmen</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Über uns</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Karriere</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Kontakt</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Partner</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Presse</a>
      </div>

       <!-- Column 5 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Rechtliches</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Datenschutz</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Nutzungsbedingungen</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Sicherheit</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Compliance</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">DSGVO</a>
      </div>

       <!-- Column 6 (Newsletter) -->
      <div class="flex flex-col gap-4 lg:col-span-1">
        <h4 class="font-semibold text-gray-900 text-sm">Newsletter</h4>
        <p class="text-sm text-gray-500">Erhalten Sie Einblicke und Updates zur Logistikautomatisierung direkt in Ihr Postfach.</p>
        <div class="flex flex-col gap-2">
           <Button variant="secondary" size="sm" class="w-full !bg-black !text-white !rounded-lg">Abonnieren</Button>
        </div>
      </div>
    </div>

    <!-- Bottom -->
    <div class="pt-8 border-t border-gray-100 flex flex-col md:flex-row justify-between items-center gap-4">
      <div class="flex items-center gap-2">
         <div class="w-6 h-6 text-primary-600">
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
         <span class="text-sm text-gray-500">© 2025 LOGAID</span>
      </div>

      <div class="flex flex-col md:flex-row items-center gap-4 text-xs text-gray-500 text-center md:text-right">
        <p class="max-w-md">
           By clicking "Accept", you agree to the use of cookies on your device or browser to enhance site navigation, analyze site usage, and assist in our marketing efforts.
        </p>
        <div class="flex gap-4">
           <Button variant="primary" size="sm" class="!text-xs !py-1 !h-8">Accept all cookies</Button>
           <Button variant="outline" size="sm" class="!text-xs !py-1 !h-8">Cookie settings</Button>
        </div>
      </div>
    </div>
    
    <div class="mt-4 flex justify-end gap-6 text-xs text-gray-500">
       <a href="#" class="hover:text-gray-900">Privacy Statement</a>
       <a href="#" class="hover:text-gray-900">Terms of Service</a>
    </div>
  </div>
</footer>
