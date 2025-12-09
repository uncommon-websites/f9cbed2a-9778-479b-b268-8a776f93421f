<script lang="ts">
  export let variant: 'primary' | 'secondary' | 'outline' | 'ghost' | 'link' = 'primary';
  export let size: 'sm' | 'md' | 'lg' = 'md';
  export let href: string | undefined = undefined;
  export let fullWidth: boolean = false;

  const baseClasses = "inline-flex items-center justify-center font-medium transition-colors focus:outline-none focus:ring-2 focus:ring-offset-2 disabled:opacity-50 disabled:pointer-events-none rounded-lg";
  
  const variants = {
    primary: "bg-primary-600 text-white hover:bg-primary-700 focus:ring-primary-500",
    secondary: "bg-gray-900 text-white hover:bg-gray-800 focus:ring-gray-900",
    outline: "border border-gray-300 bg-white text-gray-700 hover:bg-gray-50 focus:ring-primary-500",
    ghost: "hover:bg-gray-100 text-gray-700 focus:ring-gray-500",
    link: "text-primary-600 hover:underline px-0",
  };

  const sizes = {
    sm: "h-8 px-3 text-sm",
    md: "h-10 px-4 py-2 text-sm",
    lg: "h-12 px-6 text-base",
  };

  $: classes = `
    ${baseClasses}
    ${variants[variant]}
    ${sizes[size]}
    ${fullWidth ? 'w-full' : ''}
    ${$$props.class || ''}
  `;
</script>

{#if href}
  <a {href} class={classes} {...$$restProps}>
    <slot />
  </a>
{:else}
  <button class={classes} {...$$restProps}>
    <slot />
  </button>
{/if}
