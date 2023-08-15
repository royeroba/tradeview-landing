<script setup lang="ts">
import FooterBar from '@/components/FooterBar.vue'
import CardItem from '@/components/CardItem.vue'
import DownloadButtons from '@/components/DownloadButtons.vue'
import ExternalLink from '@/components/icons/ExternalLinkIcon.vue'
import CommunityIcon from '@/components/icons/CommunityIcon.vue'
import ItemA from '@/components/icons/ItemA.vue'
import ItemB from '@/components/icons/ItemB.vue'
import ItemC from '@/components/icons/ItemC.vue'
import ItemD from '@/components/icons/ItemD.vue'
import ItemE from '@/components/icons/ItemE.vue'
import ItemF from '@/components/icons/ItemF.vue'
const cardItem = [
  {
    title: 'Ideal for Beginner Clients',
    description:
      'Increase trading volumes as new traders gain comfort by following successful traders in forex markets and beyond into stocks, options, commodities, and more…',
    icon: ItemA
  },
  {
    title: 'Low Barriers to Entry',
    description:
      'CommuniTraders software is free and clients can start with just a $100 minimum investment.',
    icon: ItemB
  },
  {
    title: 'Simple Interface',
    description:
      'A simple GUI provides needed features and tools but isn’t bogged down by non-core features. This allows clients to get setup quickly and start trading.',
    icon: ItemC
  },
  {
    title: 'No Long-Term Commitments',
    description:
      'Clients can easily signup to start, change signal providers, or stop the service. There is no long-term lockup.',
    icon: ItemD
  },
  {
    title: 'Funds Safety',
    description:
      'CommuniTraders benefits from the same strong regulation and banking partners standalone Tradeview clients enjoy along with transparency and negative balance protection.',
    icon: ItemE
  },
  {
    title: 'Tradeview Runs CommuniTrader',
    description:
      'You will experience the Tradeview service you know and love, no gimmicks or hidden fees, excellent live customer support, and your dedicated account manager.',
    icon: ItemF
  }
]
</script>

<template>
  <NavBar />
  <main>
    <section id="impression">
      <div id="devices">
        <img id="devices_img" src="../assets/landing_devices.png" />
      </div>
      <div id="community">
        <CommunityIcon />
        <h1>
          Tradeview’s <strong>CommuniTraders</strong> software lets <br />
          our partners provide value-added copy <br />
          trading to their clients.
        </h1>
        <DownloadButtons />
      </div>
    </section>
    <article id="perks">
      <CardItem
        :title="item.title"
        :description="item.description"
        v-bind:key="item.title"
        v-for="item in cardItem"
      >
        <component v-bind:is="item.icon"></component>
      </CardItem>
    </article>

    <article id="quickguide">
      <div>
        <h2>Leading Edge Technology</h2>
        <p>
          Easy to use management tools, our fastest <br />
          possible execution and spreads as low as 0.0.
        </p>
        <a>Quick Guide: CommuniTraders Web User Manual <ExternalLink /></a>
      </div>
      <img alt="Quick guide photo reference" src="../assets/quick_guide.png" />
    </article>

    <article id="tryitout">

        <h1>Try CommuniTraders Now!</h1>

      <DownloadButtons />
    </article>
    <FooterBar />
  </main>
</template>

<style lang="scss" scoped>
main {
  display: block;
  width: 100%;
  height: 90%;
}

#impression {
  display: flex;
  position: static;
  width: 100%;
  height: 100%;
}

#devices {
  width: 50%;

  &_img {
    position: absolute;
    top: 0;
    height: auto;
    display: block;
    z-index: -1;
  }
}

#community {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 50%;
  height: 100%;

  h1 {
    font-size: 32px;
    font-weight: 300;
    margin-top: 10%;
    text-align: center;
    border-top: 2px solid gray;
    color: var(--vt-c-white-soft);
  }
}

#perks {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  padding: 5% 10%;
  gap: 5%;
  z-index: 1;
  background-color: var(--vt-c-white-soft);
}

.downloads {
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 1em;
  margin-top: 2em;
  width: 100%;
  &__item {
    display: flex;
    flex-direction: column;
    height: 100%;
    padding-right: 30px;
    margin-top: 2em;

    button {
      font-size: 18px;
      font-weight: bold;
      margin-top: 1em;
    }
  }

  &__item:not(:first-child) {
    border-left: 1px solid gray;
    padding-left: 30px;
  }

  &__item:last-child {
    border-left: 1px solid gray;
    padding-right: 0;
  }
}

#quickguide {
  display: flex;
  justify-content: center;
  gap: 10em;
  align-items: center;
  background-color: var(--vt-c-white-mute);
  color: var(--text-color);
  padding: 8em 4em;
  h2 {
    font-size: 30px;
    font-weight: bold;
  }

  p {
    margin-top: 1em;
    margin-bottom: 1em;
    font-size: 25px;
  }

  a {
    font-size: 18px;
    text-decoration: underline;
    cursor: pointer;
  }
}

#tryitout {
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 5% 10%;
  h1 {
    text-align: center;
    color: var(--vt-c-white-mute);
    font-size: 30px;
    font-weight: bold;
  }
}
</style>
