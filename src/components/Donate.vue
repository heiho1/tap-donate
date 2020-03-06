<template>
  <v-container>
    <v-row class="text-center panel">
      <v-col class="mb-4 panel">
        <v-img
          :src="require('../assets/img/0x8C6C1523E064eb85c78D756760dd1e70265d2A86.png')"
          class="my-3"
          contain
          height="200"
        />
        <h3>{{ msg }}</h3>
        <sub>ETH donations go to: 0x8C6C1523E064eb85c78D756760dd1e70265d2A86</sub>
        <v-alert
          max-width="20em"
          color="teal"
        >911 Truth Action Project [911 TAP] is excited to announce the launch of our TruthCoin!</v-alert>
        <v-alert max-width="20em" color="teal lighten-4">
          TruthCoin is an exchangeable and collectible Ethereum blockchain token built on the ERC20 token standard.
          The TruthCoin will be minted in a limited quantity and sent to anyone who donates Ethereum [ETH] to TAP,
          to further our common interest in the development of a society based upon truthful exchange of
          information and honest investigation of the root causes of events like the crimes of September 11, 2001.
          <v-expansion-panels :popout="true" :hover="true" :focusable="true">
            <v-expansion-panel>
              <v-expansion-panel-header>Learn More</v-expansion-panel-header>
              <v-expansion-panel-content>
                <div>
                  <p>
                    TAP is an experiment in peaceful, constitutional rebellion against the usurpation of liberties that
                    occurred immediately after 9/11. It seeks to build Truth Action Groups in every city and county to
                    redeem the faith of the Founding Fathers that Americans would not fall prey to tyranny, corruption or
                    militarism, but rather be a beacon of freedom and self-government, for and by the people, not an elite.
                    From these local groups, similar to the pre-Revolution colonial Committees of Correspondence, new
                    political structures and strategies will develop.
                  </p>

                  <p>
                    With the Truthcoin, TAP proposes to build what blockchain experts call a “distributed autonomous
                    organization” to open a new front in this campaign. As a first stage, TAP is offering introductory
                    Truthcoins to those who donate cryptocurrency to help fund TAP’s operating budget. With your
                    support, TAP will be able to hire staff for the first time; produce a regular video podcast, promote its
                    local "Truth Booth" and Truth Action Group projects, upgrade its website, and build relationships with
                    independent media, Truth-friendly blogs, and other organizations fighting against secrecy, covert
                    actions, surveillance, and kleptocratic oligarchy.
                  </p>
                  <h3>You can make a difference by volunteering and donating to the Truth Action Project.</h3>
                </div>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-alert>
        <v-btn
          href="https://911tap.org"
          target="_blank"
          rel="noopener noreferrer"
          :ripple="true"
          color="teal darken-1"
        >Join TAP today</v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import "../assets/styles/materialdesignicons.min.css"; 
import "../assets/styles/roboto.css";
import '../assets/styles/vuetify.css';

export default {
  name: "Donate",
  props: {
    msg: {
      type: String,
      default: 'A Coin for Truth'
    }
  },
  computed: {
    tapUrl() {
      return "https://911tap.org";
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.panel {
  max-width: 20em;
  max-height: 30em;
}
</style>
