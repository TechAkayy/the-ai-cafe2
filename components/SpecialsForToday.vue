<script setup lang="ts">
  // const props = defineProps({
  // 	name: {
  // 		type: String,
  // 		default: 'SpecialsForToday',
  // 	},
  // })

  // const emit = defineEmits(['addToCart'])

  // // Use the addToCart function like this:
  // // Eg-1: addToCart('pizza', 10)
  // // Eg-2: (event) => addToCart('pizza', 10, event)
  // const addToCart = (item, quantity /*, event*/) => {
  // 	emit('addToCart', { item, quantity })
  // }
</script>
<template>
  <div class="my-8">
    <section class="py-10 to-white">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold text-center mb-4">Today's Special</h2>
        <p class="text-center">
          Discover our delicious dishes and drinks tailored just for you!
        </p>
      </div>
    </section>
    <div
      class="grid gap-6 grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-3"
    >
      <v-card class="max-w-sm">
        <v-img
          src="https://images.unsplash.com/photo-1493770348161-369560ae357d?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDE3fHxmb29kfGVufDB8fHx8MTY5OTY4NjIyN3ww&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
          alt="Food 1"
          class="w-full"
        />
        <v-card-text>
          <div class="font-bold text-xl mb-2">Cheeseburger Combo</div>
          <p class="text-base">
            A juicy beef patty with melted cheese, served with crispy fries and
            a refreshing drink.
          </p>
        </v-card-text>
        <v-card-actions>
          <v-chip class="rounded-full mr-2" color="primary">$9.99</v-chip>
          <v-chip class="rounded-full" color="primary">$5.99</v-chip>
        </v-card-actions>
      </v-card>
      <v-card class="max-w-sm">
        <v-img
          src="https://images.unsplash.com/photo-1467003909585-2f8a72700288?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDEzfHxmb29kfGVufDB8fHx8MTY5OTY4NjIyN3ww&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
          alt="Food 2"
          class="w-full"
        />
        <v-card-text>
          <div class="font-bold text-xl mb-2">Pasta Carbonara</div>
          <p class="text-base">
            A classic Italian pasta dish with creamy sauce, bacon, and Parmesan
            cheese.
          </p>
        </v-card-text>
        <v-card-actions>
          <v-chip class="rounded-full mr-2" color="primary">$12.99</v-chip>
          <v-chip class="rounded-full" color="primary">$8.99</v-chip>
        </v-card-actions>
      </v-card>
      <v-card class="max-w-sm">
        <v-img
          src="https://images.unsplash.com/photo-1498837167922-ddd27525d352?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDE5fHxmb29kfGVufDB8fHx8MTY5OTY4NjIyN3ww&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
          alt="Food 3"
          class="w-full"
        />
        <v-card-text>
          <div class="font-bold text-xl mb-2">Chicken Caesar Salad</div>
          <p class="text-base">
            Fresh romaine lettuce with grilled chicken, crispy croutons, and
            tangy Caesar dressing.
          </p>
        </v-card-text>
        <v-card-actions>
          <v-chip class="rounded-full mr-2" color="primary">$10.99</v-chip>
          <v-chip class="rounded-full" color="primary">$6.99</v-chip>
        </v-card-actions>
      </v-card>
      <v-card class="max-w-sm">
        <v-img
          src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDJ8fGZvb2R8ZW58MHx8fHwxNjk5Njg2MjI3fDA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
          alt="Food 4"
          class="w-full"
        />
        <v-card-text>
          <div class="font-bold text-xl mb-2">Vegetable Curry</div>
          <p class="text-base">
            A flavorful blend of assorted vegetables cooked in a rich and spicy
            curry sauce.
          </p>
        </v-card-text>
        <v-card-actions>
          <v-chip class="rounded-full mr-2" color="primary">$11.99</v-chip>
          <v-chip class="rounded-full" color="primary">$7.99</v-chip>
        </v-card-actions>
      </v-card>
      <v-card class="max-w-sm">
        <v-img
          src="https://images.unsplash.com/photo-1695653422259-8a74ffe90401?ixid=M3wyMDkyMnwxfDF8c2VhcmNofDE1fHxmb29kfGVufDB8fHx8MTY5OTY4NjIyN3ww&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
          alt="Food 5"
          class="w-full"
        />
        <v-card-text>
          <div class="font-bold text-xl mb-2">Fish and Chips</div>
          <p class="text-base">
            Crispy battered fish served with golden fries and tartar sauce.
          </p>
        </v-card-text>
        <v-card-actions>
          <v-chip class="rounded-full mr-2" color="primary">$8.99</v-chip>
          <v-chip class="rounded-full" color="primary">$4.99</v-chip>
        </v-card-actions>
      </v-card>
      <v-card class="max-w-sm">
        <v-img
          src="https://images.unsplash.com/photo-1565958011703-44f9829ba187?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDl8fGZvb2R8ZW58MHx8fHwxNjk5Njg2MjI3fDA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop"
          alt="Food 6"
          class="w-full"
        />
        <v-card-text>
          <div class="font-bold text-xl mb-2">Mixed Berry Pancakes</div>
          <p class="text-base">
            Fluffy pancakes topped with a medley of fresh berries and maple
            syrup.
          </p>
        </v-card-text>
        <v-card-actions>
          <v-chip class="rounded-full mr-2" color="primary">$13.99</v-chip>
          <v-chip class="rounded-full" color="primary">$9.99</v-chip>
        </v-card-actions>
      </v-card>
    </div>
  </div>
</template>
<style scoped></style>
