<template>
  <v-container grid-list-md text-xs-center>
    <v-layout row wrap>
      <v-flex xs4 max-height="40em">
        <v-img
          :src="require('../assets/img/0x8C6C1523E064eb85c78D756760dd1e70265d2A86.png')"
          contain
          height="200"
        />
        <h3 style="text-align: center">{{ msg }}</h3>
        <div style="text-align: center">
          <sub>ETH donations go to:</sub>
          <sub>0x8C6C1523E064eb85c78D756760dd1e70265d2A86</sub>
        </div>
        <v-alert
          color="teal"
        >911 Truth Action Project [911 TAP] is excited to announce the launch of our TruthCoin!</v-alert>
        <div style="text-align: center">
        <v-btn
          href="https://911tap.org"
          target="_blank"
          rel="noopener noreferrer"
          :ripple="true"
          color="teal darken-1"
        >Join TAP today</v-btn>
        &nbsp;
        <v-btn
          href="https://gab.com/911tap"
          target="_blank"
          rel="noopener noreferrer"
          :ripple="true"
          color="teal darken-1"
        >Discuss on GAB!</v-btn>
        </div>
      </v-flex>
      <v-flex xs8 max-height="40em">
        <v-alert max-width="40em" color="teal lighten-4">
          <p>
            TruthCoin is an exchangeable and collectible Ethereum blockchain token built on the ERC20 token standard.
            The TruthCoin will be minted in a limited quantity and sent to anyone who donates Ethereum [ETH] to TAP,
            to further our common interest in the development of a society based upon truthful exchange of
            information and honest investigation of the root causes of events like the crimes of September 11, 2001.
          </p>
          <br />
          <p>
            TAP is an experiment in peaceful, constitutional rebellion against the usurpation of liberties that
            occurred immediately after 9/11. It seeks to build Truth Action Groups in every city and county to
            redeem the faith of the Founding Fathers that Americans would not fall prey to tyranny, corruption or
            militarism, but rather be a beacon of freedom and self-government, for and by the people, not an elite.
            From these local groups, similar to the pre-Revolution colonial Committees of Correspondence, new
            political structures and strategies will develop.
          </p>
          <v-expansion-panels :popout="true" :hover="true" :focusable="true">
            <v-expansion-panel>
              <v-expansion-panel-header>Learn More</v-expansion-panel-header>
              <v-expansion-panel-content>
                <div>
                  <p>
                    TAP’s conventional community organizing is vital, but faces sophisticated opposition from the so-called 
                    "Deep State" which exerts control over all political parties.  The citizenry has been taught to instinctively 
                    shrink from "conspiracy theorists" who point out the forbidden obvious.  The citizenry have been force-fed 
                    "learned helplessness" and so many have lost the ability to resist the smug assurances of television spokesmen 
                    and "authoritative" newspapers.   The citizenry have been distracted by the demands of earning a living in the 
                    new "gig" economy where job security disappears.   The citizenry has been made to fear the rise of unauthorized 
                    surveillance, inexplicable mass terror attacks, and misuse of police powers to punish dissenters.  
                  </p>

                  <p>
                    With the Truthcoin, TAP proposes to build what blockchain experts call a "distributed autonomous
                    organization" to open a new front in this campaign. As a first stage, TAP is offering introductory
                    Truthcoins to those who donate cryptocurrency to help fund TAP’s operating budget. With your
                    support, TAP will be able to hire staff for the first time; produce a regular video podcast, promote its
                    local "Truth Booth" and Truth Action Group projects, upgrade its website, and build relationships with
                    independent media, Truth-friendly blogs, and other organizations fighting against secrecy, covert
                    actions, surveillance, and kleptocratic oligarchy.
                  </p>

                  <p>
                    Therefore, as a new and parallel strategy, TAP proposes to build what blockchain experts call a “distributed 
                    autonomous organization” to open a new front in this peaceful democratic campaign.  As a first stage, TAP is 
                    offering introductory Truthcoins, a new cryptocurrency, to those who donate to help fund TAP’s operating budget.  
                    With these donations, TAP will transition from being an all-volunteer organization to one that is controlled by 
                    volunteers.  As funds come in, TAP will produce a regular video podcast, promote its local “Truth Booth” and 
                    Truth Action Group projects,  upgrade its website, and build relationships with independent media, Truth-friendly 
                    blogs, and other organizations fighting against secrecy, covert actions, surveillance, and kleptocratic oligarchy.  
                  </p>
                  <p>
                    In addition, leveraging the help of technology-savvy volunteers, TAP will launch, and eventually fund with 
                    cryptocurrency contributions, a larger multi-phase Truthcoin project designed to make full of the properties of 
                    open source and block chain technology.
                  </p>
                  <p>
                    The plan is to imbue Truthcoins with—
                  </p>
                    <ul>
                      <li>voting rights in a local (privacy secured) group, to elect local and district leaders and participate in policy referenda</li>
                      <li>rights to participate, as consumers and vendors, in a Truth Economy whose transactions will inject economic value into Truthcoins as a medium of exchange</li>
                      <li>rights to store, and access, secure data ranging from research findings to membership lists</li>
                      <li>rights to help create, and access, Reputation ratings of writers and publications, to help distinguish trustworthy from untrustworthy information</li>
                      <li>the right to participate, as a free citizen, in a growing association devoted to truth and transparency:  the Truth Action Project</li>
                    </ul>
                </div>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-alert>
      </v-flex>
    </v-layout>

    <v-layout row wrap>
      <v-flex xs12 text-xs-center>
        <h3 style="text-align:center">
          You can make a difference by volunteering and donating to the Truth Action Project.
        </h3>
      </v-flex>
    </v-layout>
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
