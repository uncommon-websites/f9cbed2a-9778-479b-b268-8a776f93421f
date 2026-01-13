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
  
  <!-- Feature 1: Email Classification -->
  <FeatureSection 
    title="Intelligent email classification that understands logistics"
    subtitle="AI-POWERED EMAIL ROUTING"
    linkText="See classification in action"
    bullets={[
      "Automatically categorizes quotes, bookings, tracking, and customs",
      "Routes emails to the right team or workflow instantly",
      "Learns from your specific logistics terminology",
      "Handles multiple languages and formats"
    ]}
  >
    <div slot="description">
      <p>Stop manually sorting through thousands of emails. LOGAID's AI instantly identifies email types and routes them to the correct destination.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
      <!-- Email classification mockup -->
      <div class="bg-white rounded-xl shadow-lg p-6 w-[90%] max-w-md relative">
        <div class="space-y-3">
          <div class="p-3 bg-blue-50 rounded-lg border-l-4 border-blue-500">
            <div class="flex items-center justify-between mb-1">
              <div class="text-xs font-semibold text-blue-900">Quote Request</div>
              <div class="text-xs text-blue-600">95% confidence</div>
            </div>
            <div class="text-xs text-blue-700">FCL Shanghai → Rotterdam</div>
          </div>
          
          <div class="p-3 bg-green-50 rounded-lg border-l-4 border-green-500">
            <div class="flex items-center justify-between mb-1">
              <div class="text-xs font-semibold text-green-900">Booking Confirmation</div>
              <div class="text-xs text-green-600">98% confidence</div>
            </div>
            <div class="text-xs text-green-700">Container #MSCU1234567</div>
          </div>
          
          <div class="p-3 bg-purple-50 rounded-lg border-l-4 border-purple-500">
            <div class="flex items-center justify-between mb-1">
              <div class="text-xs font-semibold text-purple-900">Tracking Update</div>
              <div class="text-xs text-purple-600">97% confidence</div>
            </div>
            <div class="text-xs text-purple-700">Vessel departed port</div>
          </div>
        </div>
        
        <!-- Floating routing indicator -->
        <div class="absolute -right-8 top-1/2 -translate-y-1/2 bg-primary-600 text-white p-2 rounded-lg shadow-md text-xs font-medium">
          Auto-routed →
        </div>
      </div>
    </div>
  </FeatureSection>

  <!-- Feature 2: AI Draft Responses -->
  <FeatureSection 
    title="AI-generated draft responses in seconds"
    subtitle="SMART EMAIL DRAFTING"
    linkText="See drafting capabilities"
    reversed={true}
    bullets={[
      "Context-aware responses using your company data",
      "Pulls real-time information from TMS and WMS",
      "Maintains your brand voice and terminology",
      "Supports 40+ languages automatically"
    ]}
  >
    <div slot="description">
      <p>Let AI handle the heavy lifting. LOGAID generates accurate, professional draft responses that your team can review and send with one click.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Email draft mockup -->
       <div class="bg-white rounded-xl shadow-lg w-[90%] overflow-hidden border border-gray-100">
         <div class="bg-gray-50 p-3 border-b border-gray-200">
            <div class="text-xs text-gray-500 mb-1">To: customer@example.com</div>
            <div class="text-xs font-semibold text-gray-900">Re: Quote Request - Shanghai to Rotterdam</div>
         </div>
         <div class="p-4 space-y-3">
            <div class="text-xs text-gray-700">Dear Customer,</div>
            <div class="text-xs text-gray-700 leading-relaxed">
               Thank you for your quote request. Based on your requirements for FCL shipment from Shanghai to Rotterdam:
            </div>
            <div class="bg-blue-50 p-3 rounded text-xs space-y-1 border border-blue-100">
               <div class="flex justify-between">
                  <span class="text-gray-600">20' Container:</span>
                  <span class="font-semibold text-gray-900">$2,450</span>
               </div>
               <div class="flex justify-between">
                  <span class="text-gray-600">40' Container:</span>
                  <span class="font-semibold text-gray-900">$3,200</span>
               </div>
               <div class="flex justify-between">
                  <span class="text-gray-600">Transit time:</span>
                  <span class="font-semibold text-gray-900">28-32 days</span>
               </div>
            </div>
            <div class="flex items-center gap-2 text-xs text-green-600 bg-green-50 p-2 rounded">
               <svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="20 6 9 17 4 12"></polyline></svg>
               Draft ready for review
            </div>
         </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 3: System Integration -->
  <FeatureSection 
    title="Deep integration with your logistics systems"
    subtitle="SEAMLESS CONNECTIVITY"
    linkText="View integrations"
    bullets={[
      "Direct integration with TMS, WMS, and ERP systems",
      "Real-time data sync for accurate responses",
      "API-first architecture for custom workflows",
      "Pre-built connectors for SAP, Oracle, and more"
    ]}
  >
    <div slot="description">
      <p>LOGAID connects directly to your existing systems, pulling real-time shipment data and updating records automatically—no manual data entry required.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Integration diagram -->
       <div class="flex flex-col items-center gap-6 w-full">
          <div class="bg-primary-600 text-white p-4 rounded-lg shadow-md font-semibold text-sm">
             LOGAID
          </div>
          
          <div class="flex gap-3">
             <div class="h-12 w-px bg-gray-300"></div>
             <div class="h-12 w-px bg-gray-300"></div>
             <div class="h-12 w-px bg-gray-300"></div>
          </div>
          
          <div class="grid grid-cols-3 gap-4 w-full max-w-md">
             <div class="bg-white p-3 rounded-lg shadow-sm border border-gray-200 text-center">
                <div class="text-xs font-semibold text-gray-900 mb-1">TMS</div>
                <div class="text-[10px] text-gray-500">CargoWise</div>
             </div>
             <div class="bg-white p-3 rounded-lg shadow-sm border border-gray-200 text-center">
                <div class="text-xs font-semibold text-gray-900 mb-1">WMS</div>
                <div class="text-[10px] text-gray-500">SAP EWM</div>
             </div>
             <div class="bg-white p-3 rounded-lg shadow-sm border border-gray-200 text-center">
                <div class="text-xs font-semibold text-gray-900 mb-1">ERP</div>
                <div class="text-[10px] text-gray-500">Oracle</div>
             </div>
          </div>
          
          <div class="bg-green-50 px-4 py-2 rounded-full text-xs text-green-700 font-medium border border-green-200">
             ✓ Real-time sync active
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 4: Analytics & Insights -->
  <FeatureSection 
    title="Actionable insights from every email interaction"
    subtitle="ANALYTICS & REPORTING"
    linkText="Explore analytics"
    reversed={true}
    bullets={[
      "Track response times and team performance",
      "Identify common customer requests and pain points",
      "Monitor classification accuracy and improve over time",
      "Export reports for compliance and auditing"
    ]}
  >
    <div slot="description">
      <p>Understand your email operations like never before. LOGAID provides detailed analytics to help you optimize workflows and improve customer service.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center px-4">
       <!-- Analytics dashboard mockup -->
       <div class="bg-white rounded-xl shadow-lg w-full p-6 space-y-4">
          <div class="grid grid-cols-2 gap-4">
             <div class="bg-blue-50 p-4 rounded-lg border border-blue-100">
                <div class="text-2xl font-bold text-blue-900">2,847</div>
                <div class="text-xs text-blue-700">Emails processed today</div>
             </div>
             <div class="bg-green-50 p-4 rounded-lg border border-green-100">
                <div class="text-2xl font-bold text-green-900">4.2 min</div>
                <div class="text-xs text-green-700">Avg. response time</div>
             </div>
          </div>
          
          <div class="space-y-2">
             <div class="text-xs font-semibold text-gray-700">Top Email Categories</div>
             <div class="space-y-2">
                <div class="flex items-center gap-2">
                   <div class="text-xs text-gray-600 w-24">Quote Requests</div>
                   <div class="flex-1 bg-gray-100 rounded-full h-2">
                      <div class="bg-primary-600 h-2 rounded-full" style="width: 45%"></div>
                   </div>
                   <div class="text-xs font-semibold text-gray-900">45%</div>
                </div>
                <div class="flex items-center gap-2">
                   <div class="text-xs text-gray-600 w-24">Tracking</div>
                   <div class="flex-1 bg-gray-100 rounded-full h-2">
                      <div class="bg-primary-600 h-2 rounded-full" style="width: 30%"></div>
                   </div>
                   <div class="text-xs font-semibold text-gray-900">30%</div>
                </div>
                <div class="flex items-center gap-2">
                   <div class="text-xs text-gray-600 w-24">Bookings</div>
                   <div class="flex-1 bg-gray-100 rounded-full h-2">
                      <div class="bg-primary-600 h-2 rounded-full" style="width: 25%"></div>
                   </div>
                   <div class="text-xs font-semibold text-gray-900">25%</div>
                </div>
             </div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 5: Multi-language Support -->
  <FeatureSection 
    title="Handle global freight communication effortlessly"
    subtitle="MULTI-LANGUAGE SUPPORT"
    linkText="See language capabilities"
    bullets={[
      "Automatic detection and translation of 40+ languages",
      "Maintains context and logistics terminology accuracy",
      "Responds in customer's preferred language",
      "Supports regional variations and industry jargon"
    ]}
  >
    <div slot="description">
      <p>Communicate with partners worldwide without language barriers. LOGAID understands and responds in multiple languages while maintaining accuracy.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center px-8">
       <!-- Multi-language email examples -->
       <div class="space-y-4 w-full">
          <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-200">
             <div class="flex items-center gap-2 mb-2">
                <div class="w-6 h-6 rounded-full bg-blue-100 flex items-center justify-center text-xs">🇬🇧</div>
                <div class="text-xs font-semibold text-gray-900">English</div>
             </div>
             <div class="text-xs text-gray-600">Quote request for container shipment...</div>
          </div>
          
          <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-200">
             <div class="flex items-center gap-2 mb-2">
                <div class="w-6 h-6 rounded-full bg-red-100 flex items-center justify-center text-xs">🇨🇳</div>
                <div class="text-xs font-semibold text-gray-900">中文</div>
             </div>
             <div class="text-xs text-gray-600">集装箱运输报价请求...</div>
          </div>
          
          <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-200">
             <div class="flex items-center gap-2 mb-2">
                <div class="w-6 h-6 rounded-full bg-yellow-100 flex items-center justify-center text-xs">🇪🇸</div>
                <div class="text-xs font-semibold text-gray-900">Español</div>
             </div>
             <div class="text-xs text-gray-600">Solicitud de cotización para envío...</div>
          </div>
          
          <div class="bg-green-50 px-4 py-2 rounded-lg text-xs text-green-700 font-medium border border-green-200 text-center">
             ✓ All processed with 95%+ accuracy
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 6: Security & Compliance -->
  <FeatureSection 
    title="Enterprise-grade security and compliance"
    subtitle="SECURITY & COMPLIANCE"
    linkText="View security details"
    reversed={true}
    bullets={[
      "SOC 2 Type II and ISO 27001 certified",
      "End-to-end encryption for all email data",
      "GDPR compliant with data residency options",
      "Role-based access control and audit logs"
    ]}
  >
    <div slot="description">
      <p>Trust LOGAID with your sensitive logistics data. We maintain the highest security standards to protect your communications and meet regulatory requirements.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Security badges grid -->
       <div class="grid grid-cols-2 gap-6">
          <div class="bg-white p-6 rounded-lg shadow-sm border border-gray-200 flex flex-col items-center text-center">
             <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center text-primary-600 mb-3">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"></rect><path d="M7 11V7a5 5 0 0 1 10 0v4"></path></svg>
             </div>
             <div class="font-bold text-sm text-gray-900">SOC 2 Type II</div>
             <div class="text-xs text-gray-500 mt-1">Certified</div>
          </div>
          
          <div class="bg-white p-6 rounded-lg shadow-sm border border-gray-200 flex flex-col items-center text-center">
             <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center text-primary-600 mb-3">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path></svg>
             </div>
             <div class="font-bold text-sm text-gray-900">ISO 27001</div>
             <div class="text-xs text-gray-500 mt-1">Certified</div>
          </div>
          
          <div class="bg-white p-6 rounded-lg shadow-sm border border-gray-200 flex flex-col items-center text-center">
             <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center text-primary-600 mb-3">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2L2 7l10 5 10-5-10-5z"></path><path d="M2 17l10 5 10-5"></path><path d="M2 12l10 5 10-5"></path></svg>
             </div>
             <div class="font-bold text-sm text-gray-900">GDPR</div>
             <div class="text-xs text-gray-500 mt-1">Compliant</div>
          </div>
          
          <div class="bg-white p-6 rounded-lg shadow-sm border border-gray-200 flex flex-col items-center text-center">
             <div class="w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center text-primary-600 mb-3">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"></path><polyline points="7.5 4.21 12 6.81 16.5 4.21"></polyline><polyline points="7.5 19.79 7.5 14.6 3 12"></polyline><polyline points="21 12 16.5 14.6 16.5 19.79"></polyline><polyline points="3.27 6.96 12 12.01 20.73 6.96"></polyline><line x1="12" y1="22.08" x2="12" y2="12"></line></svg>
             </div>
             <div class="font-bold text-sm text-gray-900">256-bit</div>
             <div class="text-xs text-gray-500 mt-1">Encryption</div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <CaseStudies />
  <Integrations />
  <Resources />
  <BottomCTA />
</main>

<Footer />

