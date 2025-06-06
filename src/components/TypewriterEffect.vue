<script setup lang="ts">
interface Props {
  text: string
  speed?: number
  delay?: number
  cursor?: boolean
  loop?: boolean
  pauseTime?: number
}

const props = withDefaults(defineProps<Props>(), {
  speed: 100,
  delay: 0,
  cursor: true,
  loop: false,
  pauseTime: 2000,
})

const displayText = ref('')
const showCursor = ref(true)
const isTyping = ref(false)
const isComplete = ref(false)

let typewriterTimeout: NodeJS.Timeout | null = null
let cursorInterval: ReturnType<typeof setInterval> | null = null

function startTypewriter() {
  displayText.value = ''
  isTyping.value = true
  isComplete.value = false

  let index = 0

  function typeNextChar() {
    if (index < props.text.length) {
      displayText.value += props.text[index]
      index++
      typewriterTimeout = setTimeout(typeNextChar, props.speed)
    }
    else {
      isTyping.value = false
      isComplete.value = true

      if (props.loop) {
        setTimeout(() => {
          eraseText()
        }, props.pauseTime)
      }
    }
  }

  function eraseText() {
    if (displayText.value.length > 0) {
      displayText.value = displayText.value.slice(0, -1)
      typewriterTimeout = setTimeout(eraseText, props.speed / 2)
    }
    else {
      setTimeout(startTypewriter, 500)
    }
  }

  setTimeout(typeNextChar, props.delay)
}

function startCursorBlink() {
  if (props.cursor) {
    cursorInterval = setInterval(() => {
      showCursor.value = !showCursor.value
    }, 530)
  }
}

onMounted(() => {
  startTypewriter()
  startCursorBlink()
})

onUnmounted(() => {
  if (typewriterTimeout) {
    clearTimeout(typewriterTimeout)
  }
  if (cursorInterval) {
    clearInterval(cursorInterval)
  }
})
</script>

<template>
  <span class="typewriter-text">
    {{ displayText }}
    <span
      v-if="cursor"
      class="typewriter-cursor"
      :class="{ 'cursor-visible': showCursor, 'cursor-hidden': !showCursor }"
    >|</span>
  </span>
</template>

<style scoped>
.typewriter-text {
  display: inline-block;
}

.typewriter-cursor {
  display: inline-block;
  transition: opacity 0.1s ease-in-out;
  font-weight: normal;
  color: currentColor;
}

.cursor-visible {
  opacity: 1;
}

.cursor-hidden {
  opacity: 0;
}
</style>
