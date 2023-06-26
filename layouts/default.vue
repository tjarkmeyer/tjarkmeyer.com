<template>
  <div id="app">
    <div class="max-w-5xl mx-auto min-h-screen">
      <AppHeader></AppHeader>
      <slot></slot>
    </div>
    <AppFooter></AppFooter>
  </div>
</template>

<script setup>
useHead({
  title: 'Tjark Meyer',
  meta: [
    {
      name: 'description',
      content:
        "Welcome to my website! I'm Tjark, a passionate Fullstack Engineer, skilled in both frontend and backend development. Explore my website to see my expertise in creating scalable, responsive web applications and implementing robust server-side functionalities. From conceptualization to deployment, I strive for clean and efficient code, leveraging my knowledge of various programming languages, frameworks, and tools. Join me on this journey of innovation and technology as I share my experiences and insights in the world of Fullstack Engineering.",
    },
  ],
})
useSeoMeta({
  title: 'Tjark Meyer',
  ogTitle: 'Tjark Meyer',
  description:
    "Welcome to my website! I'm Tjark, a passionate Fullstack Engineer, skilled in both frontend and backend development. Explore my website to see my expertise in creating scalable, responsive web applications and implementing robust server-side functionalities. From conceptualization to deployment, I strive for clean and efficient code, leveraging my knowledge of various programming languages, frameworks, and tools. Join me on this journey of innovation and technology as I share my experiences and insights in the world of Fullstack Engineering.",
  ogDescription:
    "Welcome to my website! I'm Tjark, a passionate Fullstack Engineer, skilled in both frontend and backend development. Explore my website to see my expertise in creating scalable, responsive web applications and implementing robust server-side functionalities. From conceptualization to deployment, I strive for clean and efficient code, leveraging my knowledge of various programming languages, frameworks, and tools. Join me on this journey of innovation and technology as I share my experiences and insights in the world of Fullstack Engineering.",
  ogImage: 'https://tjarkmeyer.com/images/tm.jpg',
})

const isElementScrolled = (element) => {
  const { bottom } = element.getBoundingClientRect()
  return (
    bottom * 0.95 <=
    (window.innerHeight || document.documentElement.clientHeight)
  )
}

let entries
onMounted(() => {
  entries = document.querySelectorAll('.reveal-hidden')
  window.addEventListener('scroll', () => {
    entries.forEach((entry) => {
      if (isElementScrolled(entry)) {
        entry.classList.add('show')
      } else {
        entry.classList.remove('show')
      }
    })
  })
})
</script>
