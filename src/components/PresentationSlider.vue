<template>
  <div class="h-screen relative z-10 font-sans overflow-hidden">
    <!-- Animated grid background -->
    <div class="grid-background">
      <!-- Subtle light source blobs -->
      <div class="light-blob-cyan"></div>
      <div class="light-blob-violet"></div>
    </div>

    <!-- Navigation -->
    <nav class="fixed top-6 left-1/2 transform -translate-x-1/2 z-50">
      <div class="flex items-center gap-3 card backdrop-blur-xl rounded-full px-6 py-3">
        <span class="font-mono opacity-80">{{ slideCounter }}</span>
        <div class="h-4 w-px bg-current opacity-20 mx-2"></div>
        <button @click="toggleTheme" class="theme-toggle">
          <svg width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
            <path v-show="theme === 'dark'" d="M8 12a4 4 0 1 0 0-8 4 4 0 0 0 0 8zM8 0a.5.5 0 0 1 .5.5v2a.5.5 0 0 1-1 0v-2A.5.5 0 0 1 8 0zm0 13a.5.5 0 0 1 .5.5v2a.5.5 0 0 1-1 0v-2A.5.5 0 0 1 8 13zm8-5a.5.5 0 0 1-.5.5h-2a.5.5 0 0 1 0-1h2a.5.5 0 0 1 .5.5zM3 8a.5.5 0 0 1-.5.5h-2a.5.5 0 0 1 0-1h2A.5.5 0 0 1 3 8zm10.657-5.657a.5.5 0 0 1 0 .707l-1.414 1.415a.5.5 0 1 1-.707-.708l1.414-1.414a.5.5 0 0 1 .707 0zm-9.193 9.193a.5.5 0 0 1 0 .707L3.05 13.657a.5.5 0 0 1-.707-.707l1.414-1.414a.5.5 0 0 1 .707 0zm9.193 2.121a.5.5 0 0 1-.707 0l-1.414-1.414a.5.5 0 0 1 .707-.707l1.414 1.414a.5.5 0 0 1 0 .707zM4.464 4.465a.5.5 0 0 1-.707 0L2.343 3.05a.5.5 0 1 1 .707-.707l1.414 1.414a.5.5 0 0 1 0 .708z"/>
            <path v-show="theme === 'light'" d="M6 .278a.768.768 0 0 1 .08.858 7.208 7.208 0 0 0-.878 3.46c0 4.021 3.278 7.277 7.318 7.277.527 0 1.04-.055 1.533-.16a.787.787 0 0 1 .81.316.733.733 0 0 1-.031.893A8.349 8.349 0 0 1 8.344 16C3.734 16 0 12.286 0 7.71 0 4.266 2.114 1.312 5.124.06A.752.752 0 0 1 6 .278z"/>
          </svg>
        </button>
      </div>
    </nav>

    <!-- Slides -->
    <div class="slide-container">
      <transition
        :name="slideDirection"
        mode="out-in"
        @before-enter="onBeforeEnter"
        @enter="onEnter"
        @leave="onLeave"
      >
        <component
          :is="slides[currentSlide]"
          :key="currentSlide"
          class="slide absolute inset-0"
        />
      </transition>
    </div>

    <!-- Controls -->
    <div class="fixed bottom-6 left-1/2 transform -translate-x-1/2 z-50">
      <div class="flex gap-6">
        <button @click="previousSlide" class="card backdrop-blur-xl rounded-full px-6 py-3 font-medium transition-all min-w-[120px] flex items-center justify-center gap-2">
          <ChevronLeftIcon class="w-5 h-5" />
          Prev
        </button>
        <button @click="nextSlide" class="card backdrop-blur-xl rounded-full px-6 py-3 font-medium transition-all min-w-[120px] flex items-center justify-center gap-2">
          Next
          <ChevronRightIcon class="w-5 h-5" />
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, computed, onMounted, onUnmounted } from 'vue'
import { ChevronLeftIcon, ChevronRightIcon } from '@heroicons/vue/24/outline'
import TitleSlide from './slides/TitleSlide.vue'
import MemorySystemSlide from './slides/MemorySystemSlide.vue'
import SlashCommandsSlide from './slides/SlashCommandsSlide.vue'
import SubagentsSlide from './slides/SubagentsSlide.vue'
import GitHubIntegrationSlide from './slides/GitHubIntegrationSlide.vue'
import ToolsMCPSlide from './slides/ToolsMCPSlide.vue'
import BestPracticesSlide from './slides/BestPracticesSlide.vue'
import RoadmapSlide from './slides/RoadmapSlide.vue'
import ACPSlide from './slides/ACPSlide.vue'
import CompetitiveSlide from './slides/CompetitiveSlide.vue'
import RealSuccessStoriesSlide from './slides/RealSuccessStoriesSlide.vue'
import BusinessAnalysisSlide from './slides/BusinessAnalysisSlide.vue'
import ProductManagerSlide from './slides/ProductManagerSlide.vue'
import BusinessAnalystSlide from './slides/BusinessAnalystSlide.vue'
import CTOSlide from './slides/CTOSlide.vue'
import MarketingManagerSlide from './slides/MarketingManagerSlide.vue'
import QAEngineerSlide from './slides/QAEngineerSlide.vue'
import CustomMCPSlide from './slides/CustomMCPSlide.vue'
import ContextEngineeringSlide from './slides/ContextEngineeringSlide.vue'
import ThankYouSlide from './slides/ThankYouSlide.vue'

const slides = [
  TitleSlide,
  MemorySystemSlide,
  SlashCommandsSlide,
  SubagentsSlide,
  GitHubIntegrationSlide,
  ToolsMCPSlide,
  BestPracticesSlide,
  RoadmapSlide,
  ACPSlide,
  CompetitiveSlide,
  RealSuccessStoriesSlide,
  BusinessAnalysisSlide,
  ProductManagerSlide,
  BusinessAnalystSlide,
  CTOSlide,
  MarketingManagerSlide,
  QAEngineerSlide,
  CustomMCPSlide,
  ContextEngineeringSlide,
  ThankYouSlide
]

const currentSlide = ref(parseInt(localStorage.getItem('presentationSlide')) || 0)
const theme = ref(localStorage.getItem('theme') || 'dark')
const slideDirection = ref('slide-left')
const isScrolling = ref(false)

const slideCounter = computed(() => {
  return `${String(currentSlide.value + 1).padStart(2, '0')} / ${slides.length}`
})

const goToSlide = (index) => {
  if (index >= 0 && index < slides.length) {
    currentSlide.value = index
    localStorage.setItem('presentationSlide', currentSlide.value.toString())
  }
}

const nextSlide = () => {
  slideDirection.value = 'slide-left'
  goToSlide((currentSlide.value + 1) % slides.length)
}

const previousSlide = () => {
  slideDirection.value = 'slide-right'
  goToSlide((currentSlide.value - 1 + slides.length) % slides.length)
}

const toggleTheme = () => {
  theme.value = theme.value === 'dark' ? 'light' : 'dark'
  // Use Tailwind's recommended approach
  if (theme.value === 'dark') {
    document.documentElement.classList.add('dark')
  } else {
    document.documentElement.classList.remove('dark')
  }
  // Store preference
  localStorage.setItem('theme', theme.value)
}

const handleKeydown = (e) => {
  if (e.key === 'ArrowRight' || e.key === ' ' || e.key === 'ArrowDown' || e.key === 'PageDown') {
    e.preventDefault()
    slideDirection.value = 'slide-left'
    nextSlide()
  } else if (e.key === 'ArrowLeft' || e.key === 'ArrowUp' || e.key === 'PageUp') {
    e.preventDefault()
    slideDirection.value = 'slide-right'
    previousSlide()
  }
}

const handleWheel = (e) => {
  e.preventDefault()

  // Throttle wheel events to prevent too rapid sliding
  if (isScrolling.value) return
  isScrolling.value = true

  if (e.deltaY > 0) {
    // Scrolling down - next slide
    slideDirection.value = 'slide-left'
    nextSlide()
  } else {
    // Scrolling up - previous slide
    slideDirection.value = 'slide-right'
    previousSlide()
  }

  // Reset throttle after a short delay
  setTimeout(() => {
    isScrolling.value = false
  }, 800)
}

const onBeforeEnter = (el) => {
  el.style.opacity = '0'
}

const onEnter = (el, done) => {
  el.offsetHeight // force reflow
  el.style.transition = 'all 0.5s ease-in-out'
  el.style.opacity = '1'
  setTimeout(done, 500)
}

const onLeave = (el, done) => {
  el.style.transition = 'all 0.5s ease-in-out'
  el.style.opacity = '0'
  setTimeout(done, 500)
}

const handleMouseMove = (e) => {
  const cards = document.querySelectorAll('.card')
  cards.forEach(card => {
    const rect = card.getBoundingClientRect()

    // Check if mouse is over this card
    if (e.clientX >= rect.left && e.clientX <= rect.right &&
        e.clientY >= rect.top && e.clientY <= rect.bottom) {
      const x = ((e.clientX - rect.left) / rect.width) * 100
      const y = ((e.clientY - rect.top) / rect.height) * 100

      card.style.setProperty('--mouse-x', `${x}%`)
      card.style.setProperty('--mouse-y', `${y}%`)
    }
  })
}

onMounted(() => {
  document.addEventListener('keydown', handleKeydown)
  document.addEventListener('wheel', handleWheel, { passive: false })
  document.addEventListener('mousemove', handleMouseMove)
  // Initialize theme using Tailwind's approach
  if (theme.value === 'dark') {
    document.documentElement.classList.add('dark')
  } else {
    document.documentElement.classList.remove('dark')
  }
})

onUnmounted(() => {
  document.removeEventListener('keydown', handleKeydown)
  document.removeEventListener('wheel', handleWheel)
  document.removeEventListener('mousemove', handleMouseMove)
})
</script>