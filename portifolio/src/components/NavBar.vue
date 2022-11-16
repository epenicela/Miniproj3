<template>
    <v-app-bar color="#fff" dark flat class="px-8">
        <v-col cols="1">
            <!--v-img :src="require('../assets/logo.svg')" class="my-3" contain height="20" /-->
        </v-col>
        <v-spacer text></v-spacer>
        <v-btn text @click="scroll('home')">Quem Sou Eu</v-btn>
        <v-btn text @click="scroll('about')">O que faço</v-btn>
        <v-btn text @click="scroll('hobbies')">Hobbies</v-btn>
    </v-app-bar>
</template>

<script>

export default {
  methods: {
    scroll (refName) {
      const element = document.getElementById(refName)
      element.scrollIntoView({ behavior: 'smooth' })
    }
  }

}
</script>
