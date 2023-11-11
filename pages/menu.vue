<script setup lang="ts">
  definePageMeta({
    title: 'Menu',
    description:
      'Savor the Flavors of a Decade: Indulge in our Legendary Coffee and Culinary Delights',
    navOrder: '2',
    type: 'primary',
    icon: 'i-mdi-home',
    ogImage:
      'https://images.unsplash.com/photo-1515697320591-f3eb3566bc3c?crop=entropy&cs=srgb&fm=jpg&ixid=M3wyMDkyMnwwfDF8c2VhcmNofDF8fGNhZmUlMjBtZW51fGVufDB8fHx8MTY5OTY5ODU0MHww&ixlib=rb-4.0.3&q=85', // url or local images inside public folder, for eg, ~/public/images/ogImage.png
  })

  const headers = [
    { title: 'Item', value: 'name', key: 'name' },
    { title: 'Price', value: 'price', key: 'price' },
    { title: 'Category', value: 'category', key: 'category' },
  ]
  const items = [
    { name: 'Cappuccino', price: '$3.99', category: 'Coffee' },
    { name: 'Latte', price: '$4.49', category: 'Coffee' },
    { name: 'Espresso', price: '$2.99', category: 'Coffee' },
    { name: 'Iced Coffee', price: '$4.99', category: 'Coffee' },
    { name: 'Bagel', price: '$2.49', category: 'Breakfast' },
    { name: 'Croissant', price: '$2.99', category: 'Breakfast' },
    { name: 'Avocado Toast', price: '$5.99', category: 'Breakfast' },
    { name: 'Panini', price: '$7.99', category: 'Lunch' },
    { name: 'Caesar Salad', price: '$8.99', category: 'Lunch' },
    { name: 'Margherita Pizza', price: '$11.99', category: 'Dinner' },
  ]
</script>
<template>
  <div class="container mx-auto">
    <section class="py-6">
      <div class="container mx-auto">
        <h1 class="text-4xl font-bold text-center mb-4">Our Menu</h1>
        <p class="text-center text-xl text-gray-700 mb-8">
          Explore our delicious offerings
        </p>
      </div>
    </section>
    <div class="max-w-lg mx-auto">
      <v-data-table
        :headers="headers"
        :items="items"
        item-key="name"
        items-per-page="20"
      ></v-data-table>
    </div>
  </div>
</template>
<style scoped></style>
