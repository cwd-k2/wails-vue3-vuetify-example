<script setup lang="ts">
import { ConsoleLog } from "../wailsjs/go/main/App.js";
</script>

<template>
  <v-app>
    <v-main>
      <v-app-bar rounded></v-app-bar>
      <div class="my-5 text-center">
        <h1 class="ma-5">Hello World</h1>
        <div class="ma-5">
          <v-btn
            color="primary"
            depressed
            outlined
            @click="() => ConsoleLog('Button Clicked')"
            >Button</v-btn
          >
        </div>
        <div class="ma-5">
          <v-btn icon>
            <v-icon>mdi-pencil</v-icon>
          </v-btn>
        </div>
      </div>
      <v-bottom-navigation>
        <v-btn @click="() => ConsoleLog('Heart Button Clicked')">
          <v-icon>mdi-heart</v-icon>
        </v-btn>
      </v-bottom-navigation>
    </v-main>
  </v-app>
</template>
