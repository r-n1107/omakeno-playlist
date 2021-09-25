<template>
  <v-container>
    <v-row class="text-center">

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          おまけの雑誌
        </h1>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          コーヒープレイリスト
        </h2>

        <v-row justify="center">
          <v-btn
            v-for="(next, i) in coffee"
            :key="i"
            :href="next.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ next.text }}
          </v-btn>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts">
  import Vue from 'vue'

  export default Vue.extend({
    name: 'PlayList',

    data: () => ({
      coffee: [
        {
          text: 'Spotify',
          href: 'https://music.apple.com/jp/playlist/%E3%82%B3%E3%83%BC%E3%83%92%E3%83%BC/pl.u-8aAVXLVcvR4N6r',
        },
        {
          text: 'Apple Music',
          href: 'https://music.apple.com/jp/playlist/%E3%82%B3%E3%83%BC%E3%83%92%E3%83%BC/pl.u-8aAVXLVcvR4N6r',
        },
        {
          text: 'YOUTUBE',
          href: 'https://youtube.com/playlist?list=PLFBluVa_aMydh1R0UNhbKkciiP9FdZHMj',
        },
      ],
    }),
  })
</script>
