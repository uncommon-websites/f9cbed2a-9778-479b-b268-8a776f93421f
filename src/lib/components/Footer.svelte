<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<footer class="bg-white pt-24 pb-12 border-t border-gray-100">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-8 mb-16">
      <!-- Column 1 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Marketing</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Overview</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Journeys</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Personalization</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Analytics</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Campaigns</a>
      </div>

      <!-- Column 2 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Data</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Overview</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">CDP</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Integration</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Segmentation</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Export & Sync</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Governance</a>
      </div>

      <!-- Column 3 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Automation</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Overview</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Workflows</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Content</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Approvals</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Dynamic Content</a>
      </div>

      <!-- Column 4 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Channels</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Overview</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Email</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">SMS</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Push Notifications</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">WhatsApp</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">RCS</a>
      </div>

       <!-- Column 5 -->
      <div class="flex flex-col gap-4">
        <h4 class="font-semibold text-gray-900 text-sm">Developer</h4>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Email API</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">WhatsApp API</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">SMS API</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Numbers API</a>
        <a href="#" class="text-sm text-gray-500 hover:text-gray-900">Voice API</a>
      </div>

       <!-- Column 6 (Newsletter) -->
      <div class="flex flex-col gap-4 lg:col-span-1">
        <h4 class="font-semibold text-gray-900 text-sm">Newsletter</h4>
        <p class="text-sm text-gray-500">Stay up to date with Bird through weekly updates to your inbox.</p>
        <div class="flex flex-col gap-2">
           <Button variant="secondary" size="sm" class="w-full !bg-black !text-white !rounded-lg">Sign up</Button>
        </div>
      </div>
    </div>

    <!-- Bottom -->
    <div class="pt-8 border-t border-gray-100 flex flex-col md:flex-row justify-between items-center gap-4">
      <div class="flex items-center gap-2">
         <div class="w-6 h-6 bg-primary-600 rounded flex items-center justify-center text-white">
            <svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 4s-.7 2.1-2 3.4c1.6 10-9.4 17.3-18 11.6 2.2.1 4.4-.6 6-2C3 15.5.5 9.6 3 5c2.2 2.6 5.6 4.1 9 4-.9-4.2 4-6.6 7-3.8 1.1 0 3-1.2 3-1.2z"></path></svg>
         </div>
         <span class="text-sm text-gray-500">© 2025 Bird</span>
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
