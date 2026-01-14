<script lang="ts">
  type Feature = {
    title: string
    description: string
    icon: string
  }

  type Props = {
    sectionTitle?: string
    sectionSubtitle?: string
    features: Feature[]
  }

  let { 
    sectionTitle = "Features", 
    sectionSubtitle = "",
    features 
  }: Props = $props()
</script>

<section class="py-24 bg-gray-50">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <!-- Section Header -->
    {#if sectionSubtitle}
      <div class="text-center mb-4">
        <div class="text-xs font-semibold text-gray-500 uppercase tracking-wider">
          {sectionSubtitle}
        </div>
      </div>
    {/if}
    
    <div class="text-center mb-16">
      <h2 class="text-3xl md:text-4xl font-semibold text-gray-900 leading-tight">
        {sectionTitle}
      </h2>
    </div>

    <!-- Features Grid -->
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      {#each features as feature}
        <div class="bg-white rounded-xl p-8 shadow-sm border border-gray-100 hover:shadow-md transition-shadow">
          <!-- Icon -->
          <div class="w-12 h-12 bg-primary-100 rounded-lg flex items-center justify-center text-primary-600 mb-6">
            {@html feature.icon}
          </div>
          
          <!-- Title -->
          <h3 class="text-xl font-semibold text-gray-900 mb-3">
            {feature.title}
          </h3>
          
          <!-- Description -->
          <p class="text-gray-600 leading-relaxed">
            {feature.description}
          </p>
        </div>
      {/each}
    </div>
  </div>
</section>
