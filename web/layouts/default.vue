<template>
  <div>
    <header class="border-red-600 border-t-4">
      <div class="container mx-auto">
        <div class="py-4 px-4 flex items-center justify-between">
          <div class="flex items-center">
            <LogoMark class="mr-4" />
            <LogoText />
          </div>
          <nav>
            <button class="text-lg md:hidden">Menu</button>
            <div class="hidden md:block">
              <div class="flex items-center space-between">
                <AppLink to="about">About</AppLink>
                <AppLink to="about">Contact</AppLink>
              </div>
            </div>
          </nav>
        </div>
      </div>
    </header>
    <main>
      <Nuxt />
    </main>
  </div>
</template>

<script>
import LogoMark from './../components/LogoMark.vue'
import LogoText from './../components/LogoText.vue'

export default {
  components: { LogoMark, LogoText },
}
</script>

<style>
.container {
  max-width: 48em;
}
</style>
