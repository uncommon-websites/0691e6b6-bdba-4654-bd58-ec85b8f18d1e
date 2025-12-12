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

<div class="min-h-screen bg-white text-black font-sans selection:bg-gray-200">
  <Header />

  <main class="flex flex-col items-center w-full">
    <!-- Hero Section -->
    <section class="flex flex-col items-center text-center pt-10 pb-12 px-4 max-w-4xl mx-auto">
      <h2 class="text-sm font-semibold mb-6">Palette</h2>
      
      <h1 class="text-5xl md:text-7xl font-bold tracking-tight leading-[1.1] mb-10">
        <div class="flex flex-wrap justify-center items-center gap-x-3 gap-y-2">
          <span>Discover your</span>
          <span class="inline-flex items-center justify-center w-12 h-12 md:w-16 md:h-16 bg-gray-100 rounded-2xl align-middle mx-1">
            <PaletteIcon className="w-6 h-6 md:w-8 md:h-8" />
          </span>
          <span>color</span>
        </div>
        <div class="flex flex-wrap justify-center items-center gap-x-3 gap-y-2">
          <span>season with</span>
          <span class="inline-flex items-center justify-center w-12 h-12 md:w-16 md:h-16 bg-gray-100 rounded-2xl align-middle mx-1">
            <SparkleIcon className="w-6 h-6 md:w-8 md:h-8" />
          </span>
          <span>AI</span>
        </div>
        <div class="flex flex-wrap justify-center items-center gap-x-3 gap-y-2">
          <span class="inline-flex items-center justify-center w-12 h-12 md:w-16 md:h-16 bg-gray-100 rounded-2xl align-middle mx-1">
            <StyleIcon className="w-6 h-6 md:w-8 md:h-8" />
          </span>
          <span>photo analysis</span>
        </div>
      </h1>

      <div class="mb-12">
        <Button>
          <Apple className="w-5 h-5" />
          <span class="text-base">Download for iOS</span>
        </Button>
      </div>

      <!-- Awards/Featured -->
      <div class="flex flex-wrap justify-center gap-8 md:gap-16 text-gray-400 text-[10px] md:text-xs font-medium uppercase tracking-widest">
        <div class="flex items-center gap-2">
          <Laurel className="w-6 h-12 md:w-8 md:h-16 scale-x-[-1]" />
          <div class="flex flex-col items-center leading-tight">
            <span class="text-[8px] md:text-[10px] text-gray-300 mb-0.5">As seen in</span>
            <span class="font-bold text-gray-300">Vogue</span>
          </div>
          <Laurel className="w-6 h-12 md:w-8 md:h-16" />
        </div>
        <div class="flex items-center gap-2">
          <Laurel className="w-6 h-12 md:w-8 md:h-16 scale-x-[-1]" />
          <div class="flex flex-col items-center leading-tight">
            <span class="text-[8px] md:text-[10px] text-gray-300 mb-0.5">Featured in</span>
            <span class="font-bold text-gray-300">Elle Magazine</span>
          </div>
          <Laurel className="w-6 h-12 md:w-8 md:h-16" />
        </div>
      </div>
    </section>

    <!-- Phone Showcase -->
    <section class="w-full max-w-[1000px] px-4 mb-24 relative flex justify-center">
      <!-- Background glow/shadow simulation -->
      <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[600px] h-[600px] bg-gray-100/50 rounded-full blur-3xl -z-10"></div>
      
      <!-- Phone Container -->
      <!-- Since we don't have the hand image, we'll present the phone UI in a nice frame -->
      <div class="relative w-[300px] md:w-[340px] h-[680px] md:h-[720px] transition-transform hover:scale-[1.02] duration-500">
        <PhoneUI />
      </div>
    </section>

    <!-- Features Text -->
    <section class="max-w-4xl mx-auto px-6 pb-32 space-y-24 text-center">
      <div class="space-y-6">
        <h3 class="text-3xl md:text-5xl font-bold tracking-tight leading-tight">
          Palette analyzes your natural features through AI to reveal your personal color season and the shades that make you shine
        </h3>
      </div>

      <div class="space-y-6">
        <h3 class="text-3xl md:text-5xl font-bold tracking-tight leading-tight">
          Get instant personalized recommendations for clothing, makeup, and accessories that complement your unique coloring
        </h3>
      </div>

      <div class="space-y-10">
        <h3 class="text-3xl md:text-5xl font-bold tracking-tight leading-tight">
          No more guessing or expensive consultations. Just upload a photo and discover the colors that were made for you
        </h3>
        
        <div class="pt-4">
          <Button>
            <Apple className="w-5 h-5" />
            <span class="text-base">Download for iOS</span>
          </Button>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="w-full py-12 flex flex-col items-center gap-6 text-center border-t border-gray-100 mt-auto">
      <div class="flex items-center gap-2">
        <svg width="24" height="24" viewBox="0 0 84 83" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M71.2898 70.8381C68.8072 73.3205 64.777 73.3205 62.2944 70.8381C61.1288 69.6726 60.3386 68.0462 59.4298 66.6766C56.6969 62.5611 53.8258 58.5181 50.9546 54.4883C48.4193 50.8272 45.8774 47.1727 43.3421 43.5116C42.8746 42.84 42.407 42.1683 41.9395 41.4967C44.1192 43.0046 46.2989 44.5191 48.4786 46.0336C52.68 48.9506 56.8813 51.861 61.0893 54.778C62.7883 55.9567 68.4581 59.677 69.5447 60.4343C70.1637 60.8623 70.7564 61.3232 71.2832 61.85C73.7658 64.3324 73.7658 68.3557 71.2832 70.8381H71.2898ZM40.5434 43.5116C38.0081 47.1727 35.4662 50.8272 32.9309 54.4883C30.0664 58.5181 27.1886 62.5545 24.4558 66.6766C23.547 68.0462 22.7567 69.6726 21.5911 70.8381C19.1085 73.3205 15.0784 73.3205 12.5958 70.8381C10.1132 68.3557 10.1132 64.3324 12.5958 61.85C13.1226 61.3232 13.7087 60.8623 14.3343 60.4343C15.4209 59.677 21.0907 55.9633 22.7897 54.778C26.9911 51.861 31.199 48.9506 35.4004 46.0336C37.5801 44.5257 39.7597 43.0112 41.9395 41.4967C41.4719 42.1683 41.0109 42.84 40.5434 43.5116ZM41.9395 82.9934C38.4295 82.9934 35.5847 80.1488 35.5847 76.6392C35.5847 75.8951 35.677 75.1511 35.8087 74.407C36.0457 73.1032 37.422 66.4658 37.7908 64.4312C38.7062 59.4005 39.6149 54.3632 40.5236 49.3325C40.9977 46.7249 41.4719 44.1108 41.9395 41.5033C42.0843 42.3066 42.2292 43.1165 42.3807 43.9199C43.1709 48.2987 43.9677 52.6841 44.7579 57.0629C45.5811 61.9356 46.4042 66.828 47.3854 71.6743C47.7081 73.2876 48.3008 74.993 48.3008 76.6458C48.3008 80.1554 45.456 83 41.9395 83V82.9934ZM35.4004 36.9599C31.199 34.0428 26.9911 31.1324 22.7897 28.2154C21.0907 27.0367 15.4209 23.323 14.3343 22.5657C13.7153 22.1377 13.1226 21.6702 12.5958 21.15C10.1132 18.6676 10.1132 14.6443 12.5958 12.1619C15.0784 9.67949 19.1019 9.67949 21.5911 12.1619C22.7567 13.3274 23.547 14.9538 24.4558 16.3234C27.1886 20.4389 30.0598 24.4819 32.9309 28.5117C35.4662 32.1728 38.0081 35.8273 40.5434 39.4884C41.0109 40.16 41.4785 40.8316 41.9395 41.5099C39.7597 39.9954 37.5801 38.4875 35.4004 36.973V36.9599ZM34.1096 42.9124C29.0785 43.8211 24.0409 44.7364 19.0098 45.6451C16.975 46.0138 10.3371 47.39 9.03318 47.6271C8.28905 47.7587 7.54492 47.8509 6.80079 47.8509C3.29087 47.8509 0.439453 45.0063 0.439453 41.4967C0.439453 37.9871 3.28429 35.1359 6.80079 35.1359C8.45367 35.1359 10.1593 35.7285 11.7727 36.0512C16.6194 37.0323 21.5055 37.8554 26.3786 38.6785C30.7578 39.4686 35.1436 40.2654 39.5227 41.0555C40.3327 41.2004 41.1361 41.3453 41.9395 41.4967C39.3317 41.9708 36.7174 42.4449 34.1096 42.9124ZM71.2898 21.1434C70.763 21.6702 70.1769 22.1311 69.5513 22.5591C68.4647 23.3164 62.7949 27.0302 61.0959 28.2088C56.8879 31.1258 52.6866 34.0363 48.4852 36.9533C46.3055 38.4612 44.1257 39.9756 41.946 41.4901C42.4136 40.8185 42.8811 40.1468 43.3487 39.4686C45.884 35.8075 48.4259 32.153 50.9612 28.4919C53.8258 24.4687 56.7035 20.4257 59.4364 16.3037C60.3452 14.9341 61.1354 13.3077 62.3009 12.1422C64.7836 9.65974 68.8137 9.65974 71.2964 12.1422C73.779 14.6246 73.779 18.6478 71.2964 21.1303L71.2898 21.1434ZM77.0847 47.8509C76.3406 47.8509 75.5964 47.7653 74.8523 47.6271C73.5484 47.39 66.9106 46.0138 64.8758 45.6451C59.8447 44.7364 54.807 43.8211 49.7759 42.9124C47.1681 42.4383 44.5538 41.9642 41.946 41.4967C42.756 41.3518 43.5594 41.207 44.3628 41.0555C48.742 40.2654 53.1277 39.4686 57.5069 38.6785C62.3799 37.8554 67.2728 37.0323 72.1129 36.0512C73.7263 35.7285 75.4318 35.1359 77.0847 35.1359C80.5946 35.1359 83.4395 37.9805 83.4395 41.4967C83.4395 45.0129 80.5946 47.8509 77.0847 47.8509ZM48.0769 8.58644C47.8398 9.89021 46.4635 16.5276 46.0948 18.5622C45.186 23.5929 44.2772 28.6302 43.3619 33.6609C42.8877 36.2685 42.4202 38.8826 41.946 41.4901C41.8012 40.6868 41.6563 39.8769 41.5114 39.0735C40.7212 34.6947 39.9244 30.3093 39.1341 25.9305C38.3176 21.0578 37.4879 16.1654 36.5067 11.3257C36.1774 9.71241 35.5913 8.00699 35.5913 6.35423C35.5913 2.84459 38.4361 0 41.946 0C45.456 0 48.3074 2.84459 48.3074 6.35423C48.3074 7.0983 48.2152 7.84237 48.0835 8.58644H48.0769Z" fill="black"/>
        </svg>
        <span class="font-bold text-xl tracking-tight text-gray-200">Palette</span>
      </div>
      <div class="flex flex-wrap justify-center gap-4 text-xs text-gray-400 font-medium">
        <a href="#" class="hover:text-black transition-colors">App Store</a>
        <span>•</span>
        <a href="#" class="hover:text-black transition-colors">Contact</a>
        <span>•</span>
        <a href="#" class="hover:text-black transition-colors">Instagram</a>
        <span>•</span>
        <a href="#" class="hover:text-black transition-colors">Pinterest</a>
        <span>•</span>
        <a href="#" class="hover:text-black transition-colors">Privacy policy</a>
      </div>
      <div class="text-[10px] text-gray-300">
        Discover your perfect colors
      </div>
    </footer>
  </main>
</div>


