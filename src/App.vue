<script setup lang="ts">

const slides = [
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
  {
    title: 'Card title',
    content: `This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.`,
    lastUpdated: '3 mins ago',

  },
];
</script>

<template>
  <header>
  </header>

  <main>
    <div class="container py-5">
      <swiper-container :slides-per-view="3" :space-between="10" :pagination="true" speed="500" loop="true"
        css-mode="true" :autoplay="true">
        <swiper-slide v-for="(slide, index) in slides" :key="index">
          <div class="card">
            <img :src="`https://picsum.photos/480/320?random=${index}`" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title">{{ slide.title }}</h5>
              <p class="card-text">{{ slide.content }}</p>
              <p class="card-text"><small class="text-body-secondary">Last updated {{ slide.lastUpdated }}</small></p>
            </div>
          </div>
        </swiper-slide>
      </swiper-container>
    </div>
  </main>
  <footer>

  </footer>
</template>
