<template>
  <b-container fluid>
    <h1 class="mt-3">
      Events
    </h1>
    <p>
      ComSSA regularly hosts various events. Events are generally either social events or professional development events.<br><br>

      Social events include LAN parties, laser tag, quiz nights, sundowners, pool, board game nights, ice skating, barbecues
      and various other smaller gatherings.<br><br>

      Professional development events are primarily designed to help computing and STEM students studying at Curtin.
      However, anyone with an interest in programming can attend these events and benefit from them. These events include
      industry talk sessions, workshops designed to enhance students programming skills and revision sessions for first year
      computing units.<br><br>

      Our events are listed on the ComSSA <a href="https://www.facebook.com/ComSSACurtin" target="_blank">Facebook page</a>, and announced
      on our <a href="https://discord.gg/SuwfFfjYJB" target="_blank">
        Discord.
      </a> Follow us on social media to keep up to date with
      the latest events and join our Discord to become a part of the conversation.<br><br>

      Been to an event recently? We would be eager to hear your <NuxtLink to="/events/feedback">
        feedback.
      </NuxtLink><br><br>

      Have a suggestion for a particular event? <NuxtLink to="/events/suggestions">
        Let us know.
      </NuxtLink>
    </p>

    <EventsAccordion
      name="networkingsundowner2023"
      accordion-text="Networking Sundowner - 2023"
      root-dir="events/networkingsundowner2023"
      :images="networkingsundowner2023"
    />

    <EventsAccordion
      name="s2lan2023"
      accordion-text="LAN Night S2 @ Escape Portal - 2023"
      root-dir="events/s2lan2023"
      :images="s2lan2023"
    />

    <EventsAccordion
      name="internationalsundowner2023"
      accordion-text="International Networking Sundowner - 2023"
      root-dir="events/internationalsundowner2023"
      :images="internationalsundowner2023"
    />

    <EventsAccordion
      name="hackathon2023"
      accordion-text="ComSSA Hackathon - 2023"
      root-dir="events/hackathon2023"
      :images="hackathon2023"
    />

    <EventsAccordion
      name="atr2023"
      accordion-text="The Amazing Tech Race - 2023"
      root-dir="events/atr2023"
      :images="atr2023"
    />

    <EventsAccordion
      name="tfti2023"
      accordion-text="Talks from the Industry 1 - 2023"
      root-dir="events/tfti2023"
      :images="tfti2023"
    />

    <EventsAccordion
      name="lan2023"
      accordion-text="LAN Night S1 @ Escape Portal - 2023"
      root-dir="events/lan2023"
      :images="lan2023"
    />

    <EventsAccordion
      name="boardgamesnight2023"
      accordion-text="Board Games Night - 2023"
      root-dir="events/boardgamesnight2023"
      :images="boardgamesnight2023"
    />

    <EventsAccordion
      name="grillthedepartment2023"
      accordion-text="Grill the Department - 2023"
      root-dir="events/grillthedepartment2023"
      :images="grillthedepartment2023"
    />

    <EventsAccordion
      name="guildoday2023"
      accordion-text="Guild O-Day - 2023"
      root-dir="events/guildoday2023"
      :images="guildoday2023"
    />

    <EventsAccordion
      name="boardgamesnight2022"
      accordion-text="Board Games Night - 2022"
      root-dir="events/boardgamesnight2022"
      :images="boardgamesnight2022"
    />

    <EventsAccordion
      name="grillthedepartment2022"
      accordion-text="Grill the Department - 2022"
      root-dir="events/grillthedepartment2022"
      :images="grillthedepartment2022"
    />

    <EventsAccordion
      name="guildoday2022"
      accordion-text="Guild O-Day - 2022"
      root-dir="events/guildoday2022"
      :images="guildoday2022"
    />

    <EventsAccordion
      name="hackathon2021"
      accordion-text="ComSSA x IET Hackathon - 2021"
      root-dir="events/hackathon2021"
      :images="hackathon2021"
    />

    <EventsAccordion
      name="lan2021"
      accordion-text="LAN Night @ Escape Portal - 2021"
      root-dir="events/lan2021"
      :images="lan2021"
    />

    <EventsAccordion
      name="tfti2021"
      accordion-text="Talks from the Industry 2 - 2021"
      root-dir="events/tfti2021"
      :images="tfti2021"
    />
  </b-container>
</template>

<script>
// webpack require.context requires static strings so here we are :)
const getLan2021 = () =>
    Array.from(require.context("~/assets/img/events/lan2021", true, /\.(jpg|png)$/).keys()).map(s => s.substr(2))

const getGuildODay2021 = () =>
    Array.from(require.context("~/assets/img/events/guildoday2021", true, /\.(jpg|png)$/).keys()).map(s => s.substr(2))

const getGrillTheDepartment2021 = () =>
    Array.from(require.context("~/assets/img/events/grillthedepartment2021", true, /\.(jpg|png)$/).keys()).map(s => s.substr(2))

const getTFTI2021 = () =>
    Array.from(require.context("~/assets/img/events/tfti2021", true, /\.(jpg|png)$/).keys()).map(s => s.substr(2))

const getHackathon2021 = () =>
    Array.from(require.context("~/assets/img/events/hackathon2021", true, /\.(jpg|png)$/).keys()).map(s => s.substr(2))

const getHackathon2023 = () =>
    Array.from(require.context("~/assets/img/events/hackathon2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

const getBoardGamesNight2022 = () =>
    Array.from(require.context("~/assets/img/events/boardgamesnight2022", true, /\.(jpg|png)$/).keys()).map(s => s.substr(2))

const getBoardGamesNight2023 = () =>
    Array.from(require.context("~/assets/img/events/boardgamesnight2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

const getGrillTheDepartment2022 = () =>
    Array.from(require.context("~/assets/img/events/grillthedepartment2022", true, /\.(jpg|png)$/).keys()).map(s => s.substr(2))

const getGrillTheDepartment2023 = () =>
    Array.from(require.context("~/assets/img/events/grillthedepartment2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

const getGuildODay2022 = () =>
    Array.from(require.context("~/assets/img/events/guildoday2022", true, /\.(jpg|png)$/).keys()).map(s => s.substr(2))

const getGuildODay2023 = () =>
    Array.from(require.context("~/assets/img/events/guildoday2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

const getLan2023 = () =>
    Array.from(require.context("~/assets/img/events/lan2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

const getTFTI2023 = () =>
    Array.from(require.context("~/assets/img/events/tfti2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

const getATR2023 = () =>
    Array.from(require.context("~/assets/img/events/atr2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

const getInternationalSundowner2023 = () =>
    Array.from(require.context("~/assets/img/events/internationalsundowner2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

const getS2Lan2023 = () =>
    Array.from(require.context("~/assets/img/events/s2lan2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

const getNetworkingSundowner2023 = () =>
    Array.from(require.context("~/assets/img/events/networkingsundowner2023", true, /\.(jpg|JPG|png)$/).keys()).map(s => s.substr(2))

export default {
    data () {
        return {
            lan2021: getLan2021(),
            lan2023: getLan2023(),
            s2lan2023: getS2Lan2023(),
            guildoday2021: getGuildODay2021(),
            grillthedepartment2021: getGrillTheDepartment2021(),
            tfti2021: getTFTI2021(),
            tfti2023: getTFTI2023(),
            hackathon2021: getHackathon2021(),
            hackathon2023: getHackathon2023(),
            boardgamesnight2022: getBoardGamesNight2022(),
            boardgamesnight2023: getBoardGamesNight2023(),
            grillthedepartment2022: getGrillTheDepartment2022(),
            grillthedepartment2023: getGrillTheDepartment2023(),
            guildoday2022: getGuildODay2022(),
            guildoday2023: getGuildODay2023(),
            atr2023: getATR2023(),
            internationalsundowner2023: getInternationalSundowner2023(),
            networkingsundowner2023: getNetworkingSundowner2023()
        }
    },

    head: {
        title: "Events"
    },

    mounted () { // Facebook embeds do not appear on component mount, for some reason the included script has to be reloaded
        this.$loadScript(
            "https://connect.facebook.net/en_GB/sdk.js#xfbml=1&version=v9.0"
        ).then(() => {
            this.$nextTick(() => {
                window.FB.XFBML.parse()
            })
        }).catch(() => {
        })
    }
}
</script>
