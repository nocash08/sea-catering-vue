<script setup lang="ts">
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { faBowlFood, faTruckFast, faChartPie } from "@fortawesome/free-solid-svg-icons";
import HeroImg1 from "@/assets/images/hero-img1.png";
import HeroImg2 from "@/assets/images/hero-img2.png";
import Vegetable from "@/assets/images/vegetable.jpg";
import Contact from "@/components/Contact.vue";
import Hero from "@/components/Hero.vue";
</script>

<template>
  <Hero />
  <!-- Fresh Ingredients Section -->
  <div class="py-12 md:py-20 relative overflow-hidden">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex flex-col lg:flex-row items-center relative z-10">
        <!-- Main Content -->
        <div class="w-full lg:w-1/2 lg:order-1 lg:ml-12 mt-8 lg:mt-0 relative z-10">
          <div
            class="bg-white/90 backdrop-blur-sm p-6 sm:p-8 rounded-2xl shadow-lg border border-white/20 hover:shadow-xl transition-all duration-300 mx-auto max-w-lg lg:max-w-none"
          >
            <div
              class="inline-flex items-center px-3 sm:px-4 py-1.5 sm:py-2 bg-green-100 text-green-800 text-xs sm:text-sm font-medium rounded-full mb-4 sm:mb-6 animate-fade-in-up"
              style="opacity: 0"
            >
              <span class="w-1.5 h-1.5 sm:w-2 sm:h-2 bg-green-500 rounded-full mr-2"></span>
              Fresh & Organic
            </div>
            <h1
              class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-800 mb-4 sm:mb-6 leading-tight overflow-hidden"
            >
              <div class="animate-fade-in-up" style="animation-delay: 0.1s; opacity: 0">
                <span
                  class="bg-clip-text text-transparent bg-gradient-to-r from-green-600 to-emerald-500"
                >
                  Fresh
                </span>
                Ingredients,
              </div>
              <div class="animate-fade-in-up" style="animation-delay: 0.3s; opacity: 0">
                <span class="block text-gray-800 mt-1 sm:mt-2">Healthy Meals</span>
              </div>
            </h1>
            <div class="space-y-3 animate-fade-in-up" style="animation-delay: 0.5s; opacity: 0">
              <p class="flex items-start text-base sm:text-lg text-gray-600 leading-relaxed">
                <span class="text-green-500 mr-2 mt-1">✓</span>
                <span>Fresh Produce — Crisp vegetables and ripe fruits for full flavor.</span>
              </p>
              <p class="flex items-start text-base sm:text-lg text-gray-600 leading-relaxed">
                <span class="text-green-500 mr-2 mt-1">✓</span>
                <span>Easy Recipes — Step-by-step cards with clear nutrition info.</span>
              </p>
              <p class="flex items-start text-base sm:text-lg text-gray-600 leading-relaxed">
                <span class="text-green-500 mr-2 mt-1">✓</span>
                <span>Premium Proteins — High-quality meats and sustainable seafood.</span>
              </p>
              <p class="flex items-start text-base sm:text-lg text-gray-600 leading-relaxed">
                <span class="text-green-500 mr-2 mt-1">✓</span>
                <span>Flexible Add-ons — Snacks, sides, or extra proteins your way.</span>
              </p>
              <p class="flex items-start text-base sm:text-lg text-gray-600 leading-relaxed">
                <span class="text-green-500 mr-2 mt-1">✓</span>
                <span>Eco-Friendly Packaging — Insulated and recyclable to keep food fresh.</span>
              </p>
            </div>
          </div>
        </div>

        <!-- Image Container -->
        <div class="relative w-full lg:w-1/2 px-4 sm:px-6 lg:px-8 py-8 lg:py-0">
          <div class="relative max-w-2xl mx-auto z-10">
            <!-- Main vegetable image -->
            <div
              class="relative transform transition-all duration-500 hover:scale-[1.02] animate-fade-in-up max-w-[90%] mx-auto"
              style="animation-delay: 0.7s; opacity: 0"
            >
              <div
                class="relative pb-[90%] sm:pb-[80%] md:pb-[70%] lg:pb-[80%] overflow-hidden rounded-2xl shadow-2xl"
              >
                <img
                  :src="Vegetable"
                  alt="Fresh Vegetables"
                  class="absolute inset-0 w-full h-full object-cover transform transition-transform duration-1000 hover:scale-110"
                  loading="lazy"
                />
                <!-- Overlay gradient -->
                <div
                  class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl"
                ></div>
              </div>
            </div>
          </div>

          <!-- Floating food images -->
          <div class="hidden md:block">
            <img
              :src="HeroImg1"
              class="absolute -top-35 -right-25 w-64 h-64 md:w-72 md:h-72 lg:w-80 lg:h-80 xl:w-96 xl:h-96 object-contain animate-float-slow z-20 drop-shadow-2xl"
              alt="Healthy food"
              style="animation-delay: 0.5s"
            />
            <img
              :src="HeroImg2"
              class="absolute -bottom-20 -left-5 w-32 h-36 md:w-40 md:h-44 lg:w-44 lg:h-48 xl:w-48 xl:h-52 object-contain animate-float z-20"
              alt="Fresh vegetables"
              style="animation-delay: 1s"
            />
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Features Section -->
  <div class="py-16 relative overflow-hidden">
    <div class="container mx-auto px-4 relative z-10">
      <div class="text-center max-w-3xl mx-auto mb-16">
        <h2 class="text-4xl font-bold text-gray-800 mb-4">What Makes Us Special</h2>
        <div class="w-20 h-1 bg-gradient-to-r from-green-400 to-emerald-300 mx-auto mb-6"></div>
        <p class="text-lg text-gray-600">
          Discover the unique qualities that set us apart in delivering exceptional catering
          services
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 justify-items-center gap-4">
        <div
          class="card bg-[#E7F1C5] w-full max-w-sm shadow-sm hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2"
        >
          <figure>
            <img
              src="https://images.unsplash.com/photo-1512621776951-a57141f2eefd?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80"
              alt="Meal Customization"
              class="h-48 w-full object-cover"
            />
          </figure>
          <div class="card-body">
            <div class="flex items-center gap-3 mb-2">
              <div class="text-3xl text-amber-600">
                <font-awesome-icon :icon="faBowlFood" />
              </div>
              <h2 class="card-title">
                Meal Customization
                <div class="badge bg-[#a8db27] ml-2">CUSTOM</div>
              </h2>
            </div>
            <p>
              Tailor your meals to your specific dietary needs and preferences. We offer a variety
              of options to suit every taste.
            </p>
            <div class="card-actions justify-end mt-4">
              <div class="badge badge-outline">Custom</div>
              <div class="badge badge-outline">Healthy</div>
            </div>
          </div>
        </div>

        <div
          class="card bg-[#E7F1C5] w-full max-w-sm shadow-sm hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2"
        >
          <figure>
            <img
              src="https://images.unsplash.com/photo-1606787366850-de6330128bfc?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80"
              alt="Nationwide Delivery"
              class="h-48 w-full object-cover"
            />
          </figure>
          <div class="card-body">
            <div class="flex items-center gap-3 mb-2">
              <div class="text-3xl text-amber-600">
                <font-awesome-icon :icon="faTruckFast" />
              </div>
              <h2 class="card-title">
                Nationwide Delivery
                <div class="badge bg-[#B1E79C] ml-2">DELIVER</div>
              </h2>
            </div>
            <p>
              We deliver fresh, healthy meals to all major cities across Indonesia, ensuring your
              food arrives on time and in perfect condition.
            </p>
            <div class="card-actions justify-end mt-4">
              <div class="badge badge-outline">Fast</div>
              <div class="badge badge-outline">Reliable</div>
            </div>
          </div>
        </div>

        <div
          class="card bg-[#E7F1C5] w-full max-w-sm shadow-sm hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2"
        >
          <figure>
            <img
              src="https://images.unsplash.com/photo-1498837167922-ddd27525d352?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80"
              alt="Nutritional Info"
              class="h-48 w-full object-cover"
            />
          </figure>
          <div class="card-body">
            <div class="flex items-center gap-3 mb-2">
              <div class="text-3xl text-amber-600">
                <font-awesome-icon :icon="faChartPie" />
              </div>
              <h2 class="card-title">
                Nutritional Information
                <div class="badge badge-accent ml-2">HEALTH</div>
              </h2>
            </div>
            <p>
              Detailed nutritional breakdown for every meal, helping you stay on track with your
              health and fitness goals. Know exactly what you're eating.
            </p>
            <div class="card-actions justify-end mt-4">
              <div class="badge badge-outline">Detailed</div>
              <div class="badge badge-outline">Accurate</div>
            </div>
          </div>
        </div>
      </div>
      <Contact />
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

.card {
  animation: fadeInUp 0.6s ease-out forwards;
  opacity: 0;
}

.card:nth-child(1) {
  animation-delay: 0.1s;
}
.card:nth-child(2) {
  animation-delay: 0.3s;
}
.card:nth-child(3) {
  animation-delay: 0.5s;
}
</style>
