<script setup lang="ts">
import HeroBg from "@/assets/images/hero-bg.jpg";
</script>

<template>
  <div
    class="hero min-h-screen relative overflow-hidden"
    :style="{ backgroundImage: `url(${HeroBg})` }"
  >
    <!-- Animated background overlay -->
    <div class="hero-overlay">
      <div class="absolute inset-0"></div>
    </div>

    <div class="hero-content text-neutral-content text-center relative z-10">
      <div class="max-w-2xl">
        <transition
          appear
          enter-active-class="transition-all duration-1000 ease-out"
          enter-from-class="opacity-0 translate-y-10"
          enter-to-class="opacity-100 translate-y-0"
        >
          <h1 class="mb-5 text-4xl md:text-5xl lg:text-6xl font-extrabold leading-tight">
            <span
              class="bg-clip-text text-transparent bg-gradient-to-r from-green-400 to-emerald-300"
            >
              HEALTHY
            </span>
            <span class="block md:inline">MEALS,</span>
            <span class="block">ANYTIME, ANYWHERE</span>
          </h1>
        </transition>

        <transition
          appear
          enter-active-class="transition-all duration-1000 ease-out delay-300"
          enter-from-class="opacity-0 translate-y-5"
          enter-to-class="opacity-100 translate-y-0"
        >
          <div>
            <p class="mb-5 text-lg md:text-xl text-gray-200">
              Discover customizable healthy meal plans tailored just for you. From daily menus to
              special dietary needs, SEA Catering delivers nutritious meals nationwide across
              Indonesia.
            </p>
            <p class="mb-8 text-lg text-gray-300">
              Start your healthy journey — the easy and delicious way!
            </p>
            <button
              class="btn btn-primary btn-lg transform transition-all duration-300 hover:scale-105 hover:shadow-lg"
            >
              Explore More
              <span class="ml-2">→</span>
            </button>
          </div>
        </transition>
      </div>
    </div>
  </div>
</template>

<style scoped>
/* Animation for floating elements */
@keyframes float {
  0%,
  100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}

.animate-float {
  animation: float 6s ease-in-out infinite;
}

.animate-float-slow {
  animation: float 8s ease-in-out infinite;
}
.hero-overlay {
  background: linear-gradient(135deg, rgba(0, 0, 0, 0.7) 0%, rgba(0, 0, 0, 0.5) 100%);
  backdrop-filter: blur(2px);
}

/* Animation for cards */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
