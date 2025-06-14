# Welcome to My Animated Site!

<div class="fade-in">
  <h2>Hello, world! 👋</h2>
  <p>This paragraph fades in smoothly using CSS animation.</p>
</div>

<style>
.fade-in {
  animation: fadeIn 2s ease-in-out;
  opacity: 0;
  animation-fill-mode: forwards;
  animation-delay: 0.5s;
}

@keyframes fadeIn {
  to {
    opacity: 1;
  }
}
</style>
