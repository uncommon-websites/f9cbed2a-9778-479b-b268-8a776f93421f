<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import Stats from "$lib/components/Stats.svelte";
  import Steps from "$lib/components/Steps.svelte";
  import FeatureSection from "$lib/components/FeatureSection.svelte";
  import CaseStudies from "$lib/components/CaseStudies.svelte";
  import Integrations from "$lib/components/Integrations.svelte";
  import Resources from "$lib/components/Resources.svelte";
  import BottomCTA from "$lib/components/BottomCTA.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<Header />

<main>
  <Hero />
  <Stats />
  <Steps />
  
  <!-- Feature 1: Convert signups -->
  <FeatureSection 
    title="Convert signups to active users with sophisticated onboarding flows"
    subtitle="OPTIMIZE EVERY STEP OF THE CUSTOMER JOURNEY"
    linkText="Marketing platform"
    bullets={[
      "Account creation and KYC reminders",
      "Push notifications/email reminders for account completion",
      "Message templates for every channel",
      "AI-optimized send times for higher activation rates"
    ]}
  >
    <div slot="description">
      <p>Guide new customers from account creation to first transaction with multi-step onboarding flows.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
      <!-- Mockup for onboarding flow -->
      <div class="bg-white rounded-xl shadow-lg p-6 w-[80%] max-w-sm relative">
        <div class="flex items-center gap-2 mb-4">
          <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center text-blue-600 font-bold">1</div>
          <div class="text-sm font-semibold">Create account</div>
        </div>
        <div class="space-y-3">
          <div class="h-2 bg-gray-100 rounded w-full"></div>
          <div class="h-8 bg-blue-600 rounded w-full text-white flex items-center justify-center text-sm font-medium">Create account</div>
          <div class="flex items-center gap-2 mt-4 p-3 bg-green-50 rounded-lg border border-green-100">
             <div class="w-6 h-6 bg-green-500 rounded-full flex items-center justify-center text-white text-xs">✓</div>
             <div class="text-xs text-green-800">Your verification code is 123456 - do not share this code.</div>
          </div>
        </div>
        
        <!-- Floating elements -->
        <div class="absolute -right-12 top-10 bg-white p-3 rounded-lg shadow-md flex items-center gap-2">
           <div class="w-6 h-6 bg-gray-900 rounded-full flex items-center justify-center text-white text-xs">$</div>
           <div class="text-xs font-medium">One step left!</div>
        </div>
      </div>
    </div>
  </FeatureSection>

  <!-- Feature 2: Deliver authentication -->
  <FeatureSection 
    title="Deliver authentication instantly"
    subtitle=""
    linkText="Data platform"
    reversed={true}
    bullets={[
      "Real-time OTP codes via SMS, WhatsApp, and push",
      "Authentication Journeys with automated fallbacks",
      "End-to-end encryption",
      "Compliance-ready verification templates"
    ]}
  >
    <div slot="description">
      <p>Ensure secure logins and transactions with global OTP delivery, fallback options, and end-to-end encryption.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Diagram -->
       <div class="flex flex-col items-center gap-4">
         <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-100 w-64 flex items-center gap-3">
            <div class="w-8 h-8 bg-purple-100 rounded flex items-center justify-center text-purple-600">⚡</div>
            <div class="text-sm">
               <div class="font-semibold">Trigger</div>
               <div class="text-xs text-gray-500">Customer makes a purchase</div>
            </div>
         </div>
         <div class="h-8 w-px bg-gray-300"></div>
         <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-100 w-64 flex items-center gap-3">
            <div class="w-8 h-8 bg-green-100 rounded flex items-center justify-center text-green-600">💬</div>
            <div class="text-sm">
               <div class="font-semibold">Send SMS</div>
               <div class="text-xs text-gray-500">Send verification code to...</div>
            </div>
         </div>
         <div class="h-8 w-px bg-gray-300"></div>
         <div class="bg-orange-50 p-2 rounded-full text-xs text-orange-600 font-medium px-4 border border-orange-100">
            Conditioner
         </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 3: Send transaction updates -->
  <FeatureSection 
    title="Send transaction and account updates automatically"
    subtitle=""
    linkText="Marketing automation"
    bullets={[
      "Real-time transaction confirmations via Push",
      "Low balance and overdraft alerts",
      "Multi-language and currency localization support",
      "Spending summaries and insights"
    ]}
  >
    <div slot="description">
      <p>Keep customers informed with instant, trusted notifications for every financial event.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Mobile list UI -->
       <div class="bg-white rounded-2xl shadow-lg p-4 w-64 space-y-4">
          <div class="flex items-center gap-3 p-2 hover:bg-gray-50 rounded-lg">
             <div class="w-10 h-10 bg-gray-900 rounded-lg flex items-center justify-center text-white">$</div>
             <div>
                <div class="text-xs font-bold">Transaction received</div>
                <div class="text-[10px] text-gray-500">You received $45.00 from Paul</div>
             </div>
          </div>
          <div class="flex items-center gap-3 p-2 hover:bg-gray-50 rounded-lg">
             <div class="w-10 h-10 bg-blue-600 rounded-lg flex items-center justify-center text-white">atm</div>
             <div>
                <div class="text-xs font-bold">ATM withdrawal</div>
                <div class="text-[10px] text-gray-500">$100 from Main Street ATM</div>
             </div>
          </div>
          <div class="flex items-center gap-3 p-2 hover:bg-gray-50 rounded-lg">
             <div class="w-10 h-10 bg-green-600 rounded-lg flex items-center justify-center text-white">☕</div>
             <div>
                <div class="text-xs font-bold">Starbucks Coffee</div>
                <div class="text-[10px] text-gray-500">You spent $4.95</div>
             </div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 4: Keep customers active -->
  <FeatureSection 
    title="Keep customers active and loyal"
    subtitle=""
    linkText="Marketing automation"
    reversed={true}
    bullets={[
      "Product upgrade and feature adoption nudges",
      "Automated Journeys by event",
      "Segmentation by customer value",
      "Built-in A/B testing"
    ]}
  >
    <div slot="description">
      <p>Re-engage inactive users and reward loyal ones with personalized campaigns.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Email Mockup -->
       <div class="bg-white rounded-xl shadow-lg w-[80%] overflow-hidden border border-gray-100">
          <div class="bg-gray-50 p-3 border-b border-gray-100 flex items-center gap-2">
             <div class="w-3 h-3 rounded-full bg-red-400"></div>
             <div class="w-3 h-3 rounded-full bg-yellow-400"></div>
             <div class="w-3 h-3 rounded-full bg-green-400"></div>
          </div>
          <div class="p-6">
             <div class="flex items-center gap-2 mb-4">
                <div class="w-8 h-8 bg-black rounded-full"></div>
                <div class="text-xs font-semibold">LumePay • info@lumepay.com</div>
             </div>
             <div class="text-sm font-bold mb-2">Hi <span class="bg-yellow-100 px-1 rounded text-yellow-800">{`{{FirstName}}`}</span></div>
             <p class="text-xs text-gray-500 mb-4">
                We saw you just made your first transfer abroad — welcome to the global stage!
             </p>
             <p class="text-xs text-gray-500">
                Did you know Gold members save up to 1.5% on every currency conversion?
             </p>
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 5: Understand what drives -->
  <FeatureSection 
    title="Understand what drives transactions and engagement"
    subtitle=""
    linkText="Marketing automation"
    bullets={[
      "Attribution dashboards",
      "SLA reporting",
      "Content performance reporting",
      "Optimal send-time analysis"
    ]}
  >
    <div slot="description">
      <p>Identify your highest-impact campaigns so you can invest more in what works and cut what doesn't.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center px-8">
       <!-- Chart -->
       <div class="w-full h-64 flex items-end justify-between gap-2">
          {#each [40, 60, 30, 80, 50, 70, 45, 65, 35, 55, 75, 45] as height}
             <div class="w-full bg-indigo-100 rounded-t-sm relative group">
                <div style="height: {height}%" class="absolute bottom-0 w-full bg-indigo-500 rounded-t-sm transition-all duration-500 group-hover:bg-indigo-600"></div>
                <div style="height: {height * 0.4}%" class="absolute bottom-0 w-full bg-teal-400 rounded-t-sm opacity-80"></div>
             </div>
          {/each}
       </div>
       <!-- Legend overlay -->
       <div class="absolute top-12 right-12 bg-white p-4 rounded-lg shadow-sm border border-gray-100 text-xs">
          <div class="flex justify-between gap-8 mb-1">
             <span class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-teal-400"></span> Renewed customers</span>
             <span class="font-semibold">231</span>
          </div>
          <div class="flex justify-between gap-8 mb-1">
             <span class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-indigo-500"></span> Won customers</span>
             <span class="font-semibold">431</span>
          </div>
          <div class="flex justify-between gap-8">
             <span class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-gray-300"></span> Churned customers</span>
             <span class="font-semibold">41</span>
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 6: Security -->
  <FeatureSection 
    title="Built for security, compliance, and trust"
    subtitle=""
    linkText="Marketing automation"
    reversed={true}
    bullets={[
      "ISO 27001 and SOC 2 Type II certified",
      "End-to-end encryption for all messages",
      "SLA-backed uptime and instant scaling for high-volume sends",
      "Compliance with GDPR, CCPA, LGPD, POPI, and UK Data Protection Act"
    ]}
  >
    <div slot="description">
      <p>Safeguard sensitive financial data and meet global regulatory requirements while strengthening customer confidence in your brand.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Compliance Logos Grid -->
       <div class="grid grid-cols-2 gap-8 opacity-60 grayscale">
          <div class="flex items-center gap-2 font-bold text-lg"><svg class="w-6 h-6" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2L2 7l10 5 10-5-10-5zm0 9l2.5-1.25L12 8.5l-2.5 1.25L12 11zm0 2.5l-5-2.5-5 2.5L12 22l10-8.5-5-2.5-5 2.5z"/></svg> GDPR</div>
          <div class="flex items-center gap-2 font-bold text-lg">🔒 SOC II</div>
          <div class="flex items-center gap-2 font-bold text-lg">🏥 HIPAA</div>
          <div class="flex items-center gap-2 font-bold text-lg">⭕ OAuth</div>
          <div class="flex items-center gap-2 font-bold text-lg">🌐 ISO/IEC 27001</div>
          <div class="flex items-center gap-2 font-bold text-lg">🔑 OKTA</div>
       </div>
    </div>
  </FeatureSection>

  <CaseStudies />
  <Integrations />
  <Resources />
  <BottomCTA />
</main>

<Footer />

