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
