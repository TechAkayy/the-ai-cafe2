<script setup lang="ts">
  definePageMeta({
    title: 'Our Story',
    description:
      'Serving delightful brews and bites to brighten a decade of community connections.',
    navOrder: '3',
    type: 'primary',
    icon: 'i-mdi-home',
    ogImage:
      'https://images.unsplash.com/photo-1453614512568-c4024d13c247?crop=entropy&cs=srgb&fm=jpg&ixid=M3wyMDkyMnwwfDF8c2VhcmNofDE4fHxjYWZlJTIwbGF1bmNofGVufDB8fHx8MTY5OTcwOTcwNHww&ixlib=rb-4.0.3&q=85', // url or local images inside public folder, for eg, ~/public/images/ogImage.png
  })

  const years = [
    {
      color: 'cyan',
      year: '2012',
      header: 'Serving the Community with Love',
      description:
        'Over the years, our cafe has evolved into a beloved gathering spot for the Fraser Rise community. We take pride in serving our customers with love and providing them with the best food and coffee.',
    },
    {
      color: 'green',
      year: '2014',
      header: 'Expanding our Menu',
      description:
        'To meet the growing demands of our customers, we have expanded our menu to include a wider range of delicious food options. From breakfast classics to hearty lunches, there is something for everyone at our cafe.',
    },
    {
      color: 'pink',
      year: '2017',
      header: 'Creating Memorable Experiences',
      description:
        "We believe that a great meal is about more than just the food. That's why we continuously strive to create memorable experiences for our customers. From themed events to live music performances, there is always something exciting happening at our cafe.",
    },
    {
      color: 'amber',
      year: '2019',
      header: 'Supporting Local Farmers',
      description:
        'We are committed to supporting local farmers and using fresh, high-quality ingredients in our dishes. By sourcing our ingredients locally, we not only ensure the best flavors but also contribute to the sustainability of our community.',
    },
    {
      color: 'orange',
      year: '2021',
      header: 'Continuing to Serve the Best',
      description:
        'As we enter our 10th year of serving the Fraser Rise community, our commitment to providing the best food and coffee remains unchanged. We are grateful for the continued support and look forward to many more years of serving you.',
    },
  ]
</script>
<template>
  <div class="container mx-auto">
    <section class="py-6">
      <div class="container mx-auto">
        <h2 class="font-bold mb-4 text-4xl text-center">Our Story</h2>
        <p class="mb-4 text-center text-lg">
          Welcome to our cafe, serving the best coffee and food for the last
          decade! Discover our journey and the passion behind our craft.
        </p>
      </div>
    </section>
    <section>
      <v-timeline align="start">
        <v-timeline-item
          v-for="(year, i) in years"
          :key="i"
          :dot-color="year.color"
          size="small"
        >
          <template #opposite>
            <div
              :class="`pt-1 headline font-weight-bold text-${year.color}`"
              v-text="year.year"
            ></div>
          </template>

          <div>
            <h2
              :class="`mt-n1 headline font-weight-light mb-4 text-${year.color}`"
              v-text="year.header"
            ></h2>
            <div v-text="year.description"></div>
          </div>
        </v-timeline-item>
      </v-timeline>
    </section>
  </div>
</template>
<style scoped></style>
