<template>
  <v-app>
    <v-content>
      <Donate/>
    </v-content>
  </v-app>
</template>

<script>
import Donate from './components/Donate';

export default {
  name: 'App',

  components: {
    Donate,
  },

  data: () => ({
    //
  }),
};
</script>
