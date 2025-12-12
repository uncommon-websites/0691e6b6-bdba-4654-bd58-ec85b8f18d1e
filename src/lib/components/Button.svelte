<script lang="ts">
  type Props = {
    variant?: 'primary' | 'black';
    class?: string;
  };
  
  let { variant = 'primary', class: className = '' }: Props = $props();
</script>

<button 
  class={[
    'group inline-flex items-center justify-center gap-2.5 rounded-full px-6 py-3 text-sm font-semibold tracking-tight transition-all duration-300 active:scale-[0.97]',
    variant === 'primary' ? 'bg-black text-white hover:bg-gray-900 hover:gap-3' : '',
    variant === 'black' ? 'bg-black text-white hover:bg-gray-900 hover:gap-3' : '',
    className
  ]}
>
  <slot />
</button>
