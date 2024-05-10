<template>
    <div class="bg-white p-4 rounded-lg shadow-lg">
          <div class="flex justify-center mb-4">
            <img :src="image" alt="Action Figure" class="w-64 h-64 object-cover rounded-lg">
          </div>
          <h2 class="text-xl font-semibold text-gray-800 mb-2">{{ title }}</h2>
          <p class="text-gray-600 mb-2">{{ price }}</p> 
          <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
            Pre Order
          </button>
        </div>
    </template>

<script>
export default {
    props:{
        title: String,
        price: String,
        image: String
    },
}
</script>