<template>
  <svg width="61" height="70" viewBox="0 0 61 70" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path
      class="path1"
      d="M1 25C2.99 25 7.64 23.68 13.975 21.175C19.741 18.895 23.98 18.34 27.985 17.505C32.6094 16.5409 35.98 14.34 39.985 12.175C41.8875 11.1466 43.99 10.67 44.995 10.665C49.2499 10.6438 37.04 19.96 32.18 25.815C29.1718 29.4391 28.68 33.98 28.495 45.29C28.4554 47.7108 29.98 48.32 31.15 48.825C33.5613 49.8658 38.96 50 45.455 49.67C51.2928 49.3734 53.32 43.02 56.655 38.185C57.33 37.01 57.66 36.02 58.16 35.015C58.66 34.01 59.32 33.02 60 32"
      stroke="#1E1E1E"
      stroke-width="2"
      stroke-linecap="round"
    />
    <path
      class="path2"
      d="M13 1C13 1.66 13 16.85 12.835 39.845C12.7548 51.0209 11.34 54.98 11 63.64C10.8936 66.3495 13.66 57.02 16.985 54.01C18.7625 52.4009 21.98 52 25.31 52.495C29.8788 53.1741 29.66 59.98 30.33 64.815C30.4975 66.0239 31.32 66.98 32.32 67.655C34.4156 69.0695 38.64 69 43.135 68.67C49.1043 68.2318 51.66 61.02 53.825 57.015C55.66 53.01 57.33 50.01 57.83 46.53C58 44.04 58 40.08 58 36"
      stroke="#1E1E1E"
      stroke-width="2"
      stroke-linecap="round"
    />
    <path
      class="path3"
      d="M18 31C18 30.67 18 30.34 18.495 29.84C18.99 29.34 19.98 28.68 23 27"
      stroke="#1E1E1E"
      stroke-width="2"
      stroke-linecap="round"
    />
    <path
      class="path4"
      d="M31 32C32.98 33 37.99 33.33 39.49 32.675C40.5065 32.2311 40 29.38 39.505 28.025C39.01 26.67 38.02 26.34 38.005 25.84C37.99 25.34 38.98 24.68 39.985 24.505C41.98 24.66 43.99 25 45.49 24.34C46 23.68 46 22.36 44 19"
      stroke="#1E1E1E"
      stroke-width="2"
      stroke-linecap="round"
    />
    <path
      class="path5"
      d="M40 48C40 47.34 40 45.35 40.66 43.015C41.2071 41.0793 44.99 43.66 46.655 44C47.66 42.36 48.33 40.01 50.315 38.51C51.97 38 54.94 38 58 38"
      stroke="#1E1E1E"
      stroke-width="2"
      stroke-linecap="round"
    />
  </svg>
</template>

<style scoped>
@media (prefers-reduced-motion) {
  .path1,
  .path2,
  .path3,
  .path4,
  .path5 {
    animation: none !important;
    stroke-dasharray: unset !important;
  }
}
@media print {
  .path1,
  .path2,
  .path3,
  .path4,
  .path5 {
    animation: none !important;
    stroke-dasharray: unset !important;
  }
}
@keyframes grow {
  0% {
    stroke-dashoffset: 1px;
    stroke-dasharray: 0 400px;
    opacity: 0;
  }
  5% {
    opacity: 1;
  }
  25% {
    stroke-dasharray: 400px 0;
  }
  50% {
    stroke-dasharray: 400px 0;
  }
  75% {
    stroke-dasharray: 0 400px;
    opacity: 1;
  }
  100% {
    stroke-dasharray: 0 400px;
    opacity: 0;
  }
}
@keyframes grow2 {
  0% {
    stroke-dashoffset: 1px;
    stroke-dasharray: 0 300px;
    opacity: 0;
  }
  10% {
    opacity: 1;
  }
  30% {
    stroke-dasharray: 300px 0;
  }
  55% {
    stroke-dasharray: 300px 0;
  }
  80% {
    stroke-dasharray: 0 300px;
    opacity: 1;
  }
  100% {
    stroke-dasharray: 0 300px;
    opacity: 0;
  }
}
@keyframes grow3 {
  0% {
    stroke-dashoffset: 1px;
    stroke-dasharray: 0 50px;
    opacity: 0;
  }
  15% {
    opacity: 1;
  }
  35% {
    stroke-dasharray: 50px 0;
  }
  60% {
    stroke-dasharray: 50px 0;
  }
  85% {
    stroke-dasharray: 0 50px;
    opacity: 1;
  }
  100% {
    stroke-dasharray: 0 50px;
    opacity: 0;
  }
}
@keyframes grow4 {
  0% {
    stroke-dashoffset: 1px;
    stroke-dasharray: 0 150px;
    opacity: 0;
  }
  20% {
    opacity: 1;
  }
  40% {
    stroke-dasharray: 150px 0;
  }
  65% {
    stroke-dasharray: 150px 0;
  }
  90% {
    stroke-dasharray: 0 150px;
    opacity: 1;
  }
  100% {
    stroke-dasharray: 0 150px;
    opacity: 0;
  }
}
@keyframes grow5 {
  0% {
    stroke-dashoffset: 1px;
    stroke-dasharray: 0 100px;
    opacity: 0;
  }
  25% {
    opacity: 1;
  }
  45% {
    stroke-dasharray: 100px 0;
  }
  70% {
    stroke-dasharray: 100px 0;
  }
  95% {
    stroke-dasharray: 0 100px;
    opacity: 1;
  }
  100% {
    stroke-dasharray: 0 100px;
    opacity: 0;
  }
}
.path1 {
  stroke-dashoffset: 1px;
  stroke-dasharray: 0 400px;
  animation: grow 12s ease-in-out infinite;
  transform-origin: center;
  stroke: #303030;
  animation-delay: 0s;
}
.path2 {
  stroke-dashoffset: 1px;
  stroke-dasharray: 0 300px;
  animation: grow2 12s ease-in-out infinite;
  transform-origin: center;
  stroke: #303030;
  animation-delay: 0.5s;
}
.path3 {
  stroke-dashoffset: 1px;
  stroke-dasharray: 0 50px;
  animation: grow3 12s ease-in-out infinite;
  transform-origin: center;
  stroke: #303030;
  animation-delay: 1s;
}
.path4 {
  stroke-dashoffset: 1px;
  stroke-dasharray: 0 150px;
  animation: grow4 12s ease-in-out infinite;
  transform-origin: center;
  stroke: #303030;
  animation-delay: 1.5s;
}
.path5 {
  stroke-dashoffset: 1px;
  stroke-dasharray: 0 100px;
  animation: grow5 12s ease-in-out infinite;
  transform-origin: center;
  stroke: #303030;
  animation-delay: 2s;
}
.dark .path1,
.dark .path2,
.dark .path3,
.dark .path4,
.dark .path5 {
  stroke: #fdfdfd;
}
</style>
