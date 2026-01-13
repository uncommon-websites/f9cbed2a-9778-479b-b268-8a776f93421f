<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<footer class="bg-white pt-24 pb-12 border-t border-gray-100">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-8 mb-16">
      <!-- Column 1 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Product</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Overview</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Email Classification</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">AI Drafting</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Integrations</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Analytics</a>
      </div>

      <!-- Column 2 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Solutions</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Freight Forwarders</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">3PL Providers</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Customs Brokers</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Carriers</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Warehousing</a>
      </div>

      <!-- Column 3 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Resources</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Blog</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Case Studies</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Documentation</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">API Reference</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Help Center</a>
      </div>

      <!-- Column 4 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Company</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">About Us</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Careers</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Contact</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Partners</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Press</a>
      </div>

       <!-- Column 5 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Legal</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Privacy Policy</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Terms of Service</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Security</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Compliance</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">GDPR</a>
      </div>

       <!-- Column 6 (Newsletter) -->
      <div class="flex flex-col gap-4 lg:col-span-1">
        <h4 class="font-semibold text-gray-900 text-sm">Newsletter</h4>
        <p class="text-sm text-gray-500">Get logistics automation insights and updates delivered to your inbox.</p>
        <div class="flex flex-col gap-2">
           <Button variant="secondary" size="sm" class="w-full !bg-black !text-white !rounded-lg">Subscribe</Button>
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
