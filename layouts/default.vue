<template>
  <div id="defaultLayout">
    <Navigation/>
    <div class="content">
      <nuxt />
    </div>
    <footer id="footer">I am a footer</footer>
  </div>
</template>

<style>
body #__nuxt #__layout #defaultLayout{
  display: flex;
  flex-direction: column;
  min-height: 96vh;
}
.content {
  flex: 1;
}
</style>
