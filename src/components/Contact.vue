<script setup>
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { faPhone, faEnvelope, faLocationDot } from "@fortawesome/free-solid-svg-icons";
</script>

<template>
  <!-- Contact Section -->
  <div class="py-16">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center max-w-3xl mx-auto mb-12">
        <h2 class="text-4xl font-bold text-gray-800 mb-4">Get In Touch</h2>
        <div class="w-20 h-1 bg-gradient-to-r from-green-400 to-emerald-300 mx-auto mb-6"></div>
        <p class="text-lg text-gray-600">
          Have questions or special requests? Our team is ready to assist you with any inquiries
          about our catering services.
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-6xl mx-auto">
        <!-- Contact Card 1 -->
        <div
          class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2"
        >
          <div
            class="w-16 h-16 bg-green-200 rounded-full flex items-center justify-center mx-auto mb-6"
          >
            <font-awesome-icon :icon="faPhone" class="text-2xl text-green-600" />
          </div>
          <h3 class="text-xl font-semibold mb-3">Call Us</h3>
          <p class="text-gray-600 mb-4">Available 9:00 AM - 9:00 PM, 7 days a week</p>
          <div class="space-y-2">
            <p class="text-sm text-gray-500 mt-2">
              Manager: <span class="font-medium text-gray-700">Brian</span>
            </p>
            <a
              href="tel:08123456789"
              class="text-green-600 hover:text-green-700 font-medium inline-flex items-center transition-colors"
            >
              <font-awesome-icon :icon="faPhone" class="mr-2" />
              0812 3456 789
            </a>
          </div>
        </div>

        <!-- Contact Card 2 -->
        <div
          class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2"
        >
          <div
            class="w-16 h-16 bg-green-200 rounded-full flex items-center justify-center mx-auto mb-6"
          >
            <font-awesome-icon :icon="faEnvelope" class="text-2xl text-green-600" />
          </div>
          <h3 class="text-xl font-semibold mb-3">Email Us</h3>
          <p class="text-gray-600 mb-4">We'll respond within 24 hours</p>
          <a
            href="mailto:info@seacatering.com"
            class="text-green-600 hover:text-green-700 font-medium transition-colors break-all"
          >
            info@seacatering.com
          </a>
        </div>

        <!-- Contact Card 3 -->
        <div
          class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2"
        >
          <div
            class="w-16 h-16 bg-green-200 rounded-full flex items-center justify-center mx-auto mb-6"
          >
            <font-awesome-icon :icon="faLocationDot" class="text-2xl text-green-600" />
          </div>
          <h3 class="text-xl font-semibold mb-3">Visit Us</h3>
          <p class="text-gray-600 mb-4">Our office is open Monday to Friday</p>
          <p class="text-gray-700">
            123 Ocean View St.<br />
            Jakarta Selatan, 12345
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
