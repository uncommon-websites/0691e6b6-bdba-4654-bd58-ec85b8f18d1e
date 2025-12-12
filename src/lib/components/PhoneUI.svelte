<div class="relative bg-black rounded-[3rem] p-3 w-full h-full shadow-2xl ring-1 ring-gray-900/5">
  <!-- Power Button -->
  <div class="absolute -right-[2px] top-24 w-[2px] h-12 bg-gray-800 rounded-r-md"></div>
  <!-- Volume Buttons -->
  <div class="absolute -left-[2px] top-24 w-[2px] h-8 bg-gray-800 rounded-l-md"></div>
  <div class="absolute -left-[2px] top-36 w-[2px] h-8 bg-gray-800 rounded-l-md"></div>

  <!-- Screen -->
  <div class="bg-white w-full h-full rounded-[2.5rem] overflow-hidden relative flex flex-col">
    <!-- Status Bar / Notch Area -->
    <div class="h-12 w-full flex justify-center items-start pt-2 absolute top-0 left-0 z-20">
      <div class="w-28 h-7 bg-black rounded-full flex items-center justify-center gap-2 px-3">
        <!-- Dynamic Island Content Simulation -->
        <div class="w-full h-full flex items-center justify-between opacity-0">
           <!-- Hidden content just to keep size -->
        </div>
      </div>
    </div>

    <!-- App Content -->
    <div class="flex-1 overflow-y-auto pt-12 px-6 pb-6 text-xs font-medium select-none scrollbar-hide">
      <!-- Header -->
      <div class="flex justify-between items-center mb-8 mt-2">
        <h2 class="text-2xl font-bold tracking-tight">Your Season</h2>
        <button class="text-[10px] text-gray-400 font-semibold uppercase tracking-wide">
          Share
        </button>
      </div>

      <!-- Season Result Card -->
      <div class="mb-6 p-6 bg-gradient-to-br from-gray-50 to-gray-100 rounded-3xl">
        <div class="text-center mb-4">
          <div class="text-[10px] text-gray-400 font-semibold uppercase tracking-widest mb-2">You are a</div>
          <h3 class="text-3xl font-bold tracking-tight mb-1">Soft Autumn</h3>
          <p class="text-[10px] text-gray-500 leading-relaxed">Warm, muted, and earthy tones complement your natural features</p>
        </div>
        
        <!-- Color Palette -->
        <div class="grid grid-cols-6 gap-2 mt-4">
          <div class="aspect-square rounded-lg" style="background-color: #8B7355;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #A0826D;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #C9A87C;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #B85C4E;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #7A5C4E;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #5D6C5D;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #D4A574;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #9B6B4F;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #BC8B5C;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #8B6F47;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #A68B6A;"></div>
          <div class="aspect-square rounded-lg" style="background-color: #7B8B7A;"></div>
        </div>
      </div>

      <!-- Best Colors Section -->
      <div class="mb-6">
        <h4 class="text-xs font-bold mb-3 text-gray-900">Your Best Colors</h4>
        <div class="space-y-3">
          <div class="flex items-center gap-3">
            <div class="w-10 h-10 rounded-xl flex-shrink-0" style="background-color: #8B7355;"></div>
            <div class="flex-1">
              <div class="text-sm font-semibold">Warm Taupe</div>
              <div class="text-[10px] text-gray-400">Perfect for everyday wear</div>
            </div>
          </div>
          <div class="flex items-center gap-3">
            <div class="w-10 h-10 rounded-xl flex-shrink-0" style="background-color: #B85C4E;"></div>
            <div class="flex-1">
              <div class="text-sm font-semibold">Terracotta</div>
              <div class="text-[10px] text-gray-400">Great for statement pieces</div>
            </div>
          </div>
          <div class="flex items-center gap-3">
            <div class="w-10 h-10 rounded-xl flex-shrink-0" style="background-color: #5D6C5D;"></div>
            <div class="flex-1">
              <div class="text-sm font-semibold">Sage Green</div>
              <div class="text-[10px] text-gray-400">Complements your undertones</div>
            </div>
          </div>
        </div>
      </div>

      <!-- CTA Button -->
      <button class="w-full bg-black text-white rounded-full py-3.5 text-sm font-semibold mt-4">
        View Full Color Guide
      </button>
    </div>
    
    <!-- Home Indicator -->
    <div class="absolute bottom-1 left-1/2 -translate-x-1/2 w-32 h-1 bg-black rounded-full opacity-20"></div>
  </div>
</div>

