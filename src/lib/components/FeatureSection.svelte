<script lang="ts">
  export let title: string;
  export let subtitle: string = "";
  export let linkText: string = "";
  export let linkHref: string = "#";
  export let reversed: boolean = false;
  export let bullets: string[] = [];
</script>

<section class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex flex-col gap-16 {reversed ? 'md:flex-row-reverse' : 'md:flex-row'} items-center">
      
      <!-- Content -->
      <div class="flex-1">
        <div class="text-xs font-semibold text-gray-500 uppercase tracking-wider mb-4">{subtitle}</div>
        <h2 class="text-3xl md:text-4xl font-semibold text-gray-900 mb-6 leading-tight">
          {title}
        </h2>
        
        <div class="text-gray-500 mb-8 space-y-4">
          <slot name="description" />
        </div>

        {#if bullets.length > 0}
          <ul class="space-y-3 mb-8">
            {#each bullets as bullet}
              <li class="flex items-start gap-3 text-sm text-gray-600">
                <div class="w-1.5 h-1.5 rounded-full bg-primary-600 mt-1.5 shrink-0"></div>
                {bullet}
              </li>
            {/each}
          </ul>
        {/if}

        {#if linkText}
          <a href={linkHref} class="text-sm font-medium text-primary-600 hover:text-primary-700 flex items-center gap-1">
            {linkText}
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"></path><path d="m12 5 7 7-7 7"></path></svg>
          </a>
        {/if}
      </div>

      <!-- Visual -->
      <div class="flex-1 w-full">
        <div class="bg-gray-50 rounded-2xl p-8 md:p-12 w-full h-full min-h-[400px] flex items-center justify-center overflow-hidden relative">
          <slot name="visual" />
        </div>
      </div>

    </div>
  </div>
</section>
