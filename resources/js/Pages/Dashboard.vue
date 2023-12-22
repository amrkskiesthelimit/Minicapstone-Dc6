<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';

</script>

<template>
    <Head title="Dashboard" />

    <AuthenticatedLayout>
      <div class="py-12 fade-in">
        <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
          <div class="bg-white dark:bg-gray-800 overflow-hidden shadow-sm sm:rounded-lg">

            <!-- Header -->
            <div class="p-6 text-gray-900 dark:text-gray-100">
              <h2 class="text-2xl font-semibold">Shoes Dashboard</h2>
              <p class="mt-2 text-gray-600 dark:text-gray-400">Manage your shoe collection here.</p>
            </div>

            <hr>

            <!-- Content for Shoes -->
            <div class="p-6 text-gray-900 dark:text-gray-100 grid grid-cols-1 ">
              <!-- Add your shoe-related content here -->
              <!-- Example: Display a list of shoes -->
              <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6 mt-4">
                <!-- Shoe Card -->
                <div class="bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-800 rounded-lg p-4 transition-transform transform hover:scale-105">
                  <img src="data:image/jpeg;base64,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" alt="Shoe" class="w-full h-32 object-cover mb-2">
                  <h3 class="text-lg font-semibold">Shoe Name</h3>
                  <p class="text-gray-600 dark:text-gray-400">Brand: Nike</p>
                  <p class="text-gray-600 dark:text-gray-400">Price: $100</p>
                  <button class="bg-indigo-600 text-white px-3 py-1 rounded mt-2">Details</button>
                </div>


              </div>
              <div class="grid grid-cols-2 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6 mt-4">
                <!-- Shoe Card -->
                <div class="bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-800 rounded-lg p-4 transition-transform transform hover:scale-105">
                  <img src="data:image/jpeg;base64,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" alt="Shoe" class="w-full h-32 object-cover mb-2">
                  <h3 class="text-lg font-semibold">Shoe Name</h3>
                  <p class="text-gray-600 dark:text-gray-400">Brand: Nike Air</p>
                  <p class="text-gray-600 dark:text-gray-400">Price: $200</p>
                  <button class="bg-indigo-600 text-white px-3 py-1 rounded mt-2">Details</button>
                </div>


              </div>
            </div>
          </div>
        </div>
      </div>
    </AuthenticatedLayout>
  </template>

<style>
    @keyframes fadeIn {
        from {
            opacity: 0;
        }
        to {
            opacity: 1;
        }
    }

    .fade-in {
        animation: fadeIn 0.3s ease-in-out; /* Adjust the duration and timing function as needed */
    }
</style>
