<template>
  <div class="banner">
    <v-container>
      <h1>Home</h1>
      <v-hover v-slot="{ hover }">
        <transition name="slideLeft">
          <div v-if="hover" class="primary" style="height: 64px">a</div>
        </transition>
        <transition name="slideRight">
          <div v-if="!hover" class="primary" style="height: 64px">a</div>
        </transition>
      </v-hover>
      <transition name="slideLeft">
        <div v-if="animate" class="primary" style="height: 64px">a</div>
      </transition>
      <transition name="slideRight">
        <div v-if="!animate" class="primary" style="height: 64px">a</div>
      </transition>
      <v-btn @click="animate = !animate">animate</v-btn>

      <div class="a-slide-x-transition">
        a
      </div>
      <v-hover v-slot="{ hover }">
        <transition name="slideRight">
          <div v-if="hover" class="mt-5 orange">
            a
          </div>
          <div v-else class="mt-5 yellow">
            b
          </div>
        </transition>

      </v-hover>

    </v-container>
  </div>
</template>

<script>
export default {
  name: 'Banner',
  data: () => ({
    animate: false
  }),
  components: {}
}
</script>

<style>
.a-slide-x-transition {
  width: 600px;
  height: 64px;
  border: none;
  color: white;
  opacity: 1;
  background-color: blue;
  border-radius: 4px;
  box-shadow: inset 0 0 0 0.1px orange;
  transition: all ease 0.5s;
  outline: none;
}

.a-slide-x-transition:hover {
  box-shadow: inset 600px 0 0 0 orange;
  color: aquamarine;
  opacity: 0.5;
}

</style>
