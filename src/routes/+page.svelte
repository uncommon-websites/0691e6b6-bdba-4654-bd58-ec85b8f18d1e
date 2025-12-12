<script lang="ts">
  import Header from '$lib/components/Header.svelte';
  import Button from '$lib/components/Button.svelte';
  import Apple from '$lib/components/icons/Apple.svelte';
  import PaletteIcon from '$lib/components/icons/PaletteIcon.svelte';
  import SparkleIcon from '$lib/components/icons/SparkleIcon.svelte';
  import StyleIcon from '$lib/components/icons/StyleIcon.svelte';
  import Laurel from '$lib/components/icons/Laurel.svelte';
  import PhoneUI from '$lib/components/PhoneUI.svelte';
</script>

<svelte:head>
  <title>Palette - Discover Your Color Season with AI</title>
  <meta name="description" content="Discover your personal color season through AI photo analysis. Get personalized style guidance and find the perfect colors for your natural features." />
</svelte:head>

<div class="min-h-screen bg-gradient-to-b from-white via-gray-50/30 to-white text-black font-sans selection:bg-gray-200">
  <Header />

  <main class="flex flex-col items-center w-full">
    <!-- Hero Section -->
    <section class="flex flex-col items-center text-center pt-16 pb-20 px-4 max-w-5xl mx-auto">
      <div class="inline-flex items-center gap-2 mb-8 px-4 py-2 rounded-full bg-gray-50 border border-gray-100">
        <span class="text-xs font-medium tracking-wide text-gray-600">Palette</span>
      </div>
      
      <h1 class="text-6xl md:text-8xl font-bold tracking-[-0.02em] leading-[0.95] mb-14 text-balance">
        <div class="flex flex-wrap justify-center items-center gap-x-4 gap-y-3 mb-2">
          <span class="animate-[fadeIn_0.6s_ease-out]">Discover your</span>
          <span class="inline-flex items-center justify-center w-14 h-14 md:w-20 md:h-20 bg-gradient-to-br from-gray-50 to-gray-100 rounded-3xl align-middle transition-transform duration-500 hover:scale-110 hover:rotate-6 animate-[fadeIn_0.6s_ease-out_0.1s_both]">
            <PaletteIcon className="w-7 h-7 md:w-10 md:h-10" />
          </span>
          <span class="animate-[fadeIn_0.6s_ease-out_0.2s_both]">color</span>
        </div>
        <div class="flex flex-wrap justify-center items-center gap-x-4 gap-y-3 mb-2">
          <span class="animate-[fadeIn_0.6s_ease-out_0.3s_both]">season with</span>
          <span class="inline-flex items-center justify-center w-14 h-14 md:w-20 md:h-20 bg-gradient-to-br from-gray-50 to-gray-100 rounded-3xl align-middle transition-transform duration-500 hover:scale-110 hover:rotate-6 animate-[fadeIn_0.6s_ease-out_0.4s_both]">
            <SparkleIcon className="w-7 h-7 md:w-10 md:h-10" />
          </span>
          <span class="animate-[fadeIn_0.6s_ease-out_0.5s_both]">AI</span>
        </div>
        <div class="flex flex-wrap justify-center items-center gap-x-4 gap-y-3">
          <span class="inline-flex items-center justify-center w-14 h-14 md:w-20 md:h-20 bg-gradient-to-br from-gray-50 to-gray-100 rounded-3xl align-middle transition-transform duration-500 hover:scale-110 hover:rotate-6 animate-[fadeIn_0.6s_ease-out_0.6s_both]">
            <StyleIcon className="w-7 h-7 md:w-10 md:h-10" />
          </span>
          <span class="animate-[fadeIn_0.6s_ease-out_0.7s_both]">photo analysis</span>
        </div>
      </h1>

      <div class="mb-16 animate-[fadeIn_0.6s_ease-out_0.8s_both]">
        <Button>
          <Apple className="w-5 h-5" />
          <span class="text-base">Download for iOS</span>
        </Button>
      </div>

      <!-- Awards/Featured -->
      <div class="flex flex-wrap justify-center gap-12 md:gap-20 text-gray-400 text-[10px] md:text-xs font-medium uppercase tracking-[0.15em] animate-[fadeIn_0.6s_ease-out_0.9s_both]">
        <div class="flex items-center gap-3 transition-all duration-300 hover:scale-105">
          <Laurel className="w-6 h-12 md:w-8 md:h-16 scale-x-[-1] opacity-40" />
          <div class="flex flex-col items-center leading-tight">
            <span class="text-[8px] md:text-[10px] text-gray-400 mb-1">As seen in</span>
            <span class="font-bold text-gray-500">Vogue</span>
          </div>
          <Laurel className="w-6 h-12 md:w-8 md:h-16 opacity-40" />
        </div>
        <div class="flex items-center gap-3 transition-all duration-300 hover:scale-105">
          <Laurel className="w-6 h-12 md:w-8 md:h-16 scale-x-[-1] opacity-40" />
          <div class="flex flex-col items-center leading-tight">
            <span class="text-[8px] md:text-[10px] text-gray-400 mb-1">Featured in</span>
            <span class="font-bold text-gray-500">Elle Magazine</span>
          </div>
          <Laurel className="w-6 h-12 md:w-8 md:h-16 opacity-40" />
        </div>
      </div>
    </section>

    <!-- Phone Showcase -->
    <section class="w-full max-w-[1200px] px-4 mb-32 relative flex justify-center py-20">
      <!-- Sophisticated background effects -->
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[700px] h-[700px] bg-gradient-radial from-gray-100/60 via-gray-50/30 to-transparent rounded-full blur-3xl -z-10 animate-pulse-slow"></div>
      <div class="absolute top-1/3 left-1/3 -translate-x-1/2 -translate-y-1/2 w-[500px] h-[500px] bg-gradient-radial from-gray-50/40 to-transparent rounded-full blur-2xl -z-10"></div>
      
      <!-- Phone Container with elegant presentation -->
      <div class="relative w-[300px] md:w-[360px] h-[680px] md:h-[740px] transition-all duration-700 hover:scale-[1.03] hover:-translate-y-2">
        <div class="absolute inset-0 bg-gradient-to-b from-transparent via-gray-50/20 to-transparent rounded-[3rem] opacity-0 hover:opacity-100 transition-opacity duration-500"></div>
        <PhoneUI />
      </div>
    </section>

    <!-- Features Text -->
    <section class="max-w-5xl mx-auto px-6 pb-40 space-y-32 text-center">
      <div class="space-y-8 opacity-0 animate-[fadeIn_0.8s_ease-out_0.2s_both]">
        <h3 class="text-4xl md:text-6xl font-bold tracking-[-0.02em] leading-[1.15] text-balance text-gray-900">
          Palette analyzes your natural features through AI to reveal your personal color season and the shades that make you shine
        </h3>
        <div class="w-16 h-0.5 bg-gradient-to-r from-transparent via-gray-300 to-transparent mx-auto"></div>
      </div>

      <div class="space-y-8 opacity-0 animate-[fadeIn_0.8s_ease-out_0.4s_both]">
        <h3 class="text-4xl md:text-6xl font-bold tracking-[-0.02em] leading-[1.15] text-balance text-gray-900">
          Get instant personalized recommendations for clothing, makeup, and accessories that complement your unique coloring
        </h3>
        <div class="w-16 h-0.5 bg-gradient-to-r from-transparent via-gray-300 to-transparent mx-auto"></div>
      </div>

      <div class="space-y-12 opacity-0 animate-[fadeIn_0.8s_ease-out_0.6s_both]">
        <h3 class="text-4xl md:text-6xl font-bold tracking-[-0.02em] leading-[1.15] text-balance text-gray-900">
          No more guessing or expensive consultations. Just upload a photo and discover the colors that were made for you
        </h3>
        
        <div class="pt-6">
          <Button>
            <Apple className="w-5 h-5" />
            <span class="text-base">Download for iOS</span>
          </Button>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="w-full py-16 flex flex-col items-center gap-8 text-center border-t border-gray-100 mt-auto bg-gradient-to-b from-transparent to-gray-50/30">
      <div class="font-bold text-2xl tracking-[-0.02em] text-gray-300">Palette</div>
      <div class="flex flex-wrap justify-center gap-6 text-sm text-gray-500 font-medium">
        <a href="#" class="hover:text-black transition-all duration-300 hover:scale-105">App Store</a>
        <span class="text-gray-300">•</span>
        <a href="#" class="hover:text-black transition-all duration-300 hover:scale-105">Contact</a>
        <span class="text-gray-300">•</span>
        <a href="#" class="hover:text-black transition-all duration-300 hover:scale-105">Instagram</a>
        <span class="text-gray-300">•</span>
        <a href="#" class="hover:text-black transition-all duration-300 hover:scale-105">Pinterest</a>
        <span class="text-gray-300">•</span>
        <a href="#" class="hover:text-black transition-all duration-300 hover:scale-105">Privacy policy</a>
      </div>
      <div class="text-xs text-gray-400 tracking-wide">
        Discover your perfect colors
      </div>
    </footer>
  </main>
</div>


