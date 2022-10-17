<template>
  <q-page
    style="
      background-image: url('https://wallpaperaccess.com/full/313428.jpg');
      background-size: cover;
    "
  >
    <template>
      <div>
        <div class="q-gutter-sm">
          <q-bar dense class="bg-red-10 text-black">
            <div>Your app is Running</div>
            <q-icon name="check" />
            <q-space />
            <q-icon name="bluetooth" />
            <q-icon name="signal_wifi_4_bar" />
            <q-icon name="signal_cellular_4_bar" />
            <div class="gt-xs">100%</div>
            <q-icon name="battery_full" />
            <div>10:00AM</div>
          </q-bar>
        </div>

        <div class="q-pa-sm">
          <div class="bg-red-10 text-black">
            <q-toolbar>
              <q-btn flat round dense icon="assignment_ind" />
              <q-toolbar-title>All Red Dead Info</q-toolbar-title>
              <q-btn flat round dense icon="gamepad" class="q-mr-xs" />
              <q-btn flat round dense icon="web" @click="dialog = true" />
              <q-dialog v-model="dialog">
                <q-card class="bg-red-10">
                  <q-card-section>
                    <div style="color: white" class="text-h6 flex flex-center">
                      Info
                    </div>
                  </q-card-section>

                  <q-card-section class="q-pt-none">
                    The world of Red Dead Redemption 2 spans five fictitious
                    U.S. states. The states of New Hanover, Ambarino, and
                    Lemoyne are new to the series, and are located to the
                    immediate north and east of Red Dead Redemption's world,
                    whilst the states of New Austin and West Elizabeth return
                    from Red Dead Redemption. The states are centered on the San
                    Luis and Lannahechee Rivers and the shores of Flat Iron
                    Lake. Ambarino is a mountain wilderness, with the largest
                    settlement being the Wapiti Native American reservation; New
                    Hanover encompasses a sweeping valley and woody foothills
                    that feature the cattle town of Valentine, the riverside Van
                    Horn Trading Post, and the coal town of Annesburg; and
                    Lemoyne is composed of bayous and plantations resembling the
                    southeastern United States, and is home to the Southern town
                    of Rhodes, the village of Lagras, and the former French
                    colony of Saint Denis, analogous to New Orleans. West
                    Elizabeth consists of wide plains, dense forests, and the
                    prosperous port town of Blackwater. This region has been
                    expanded from the original Red Dead Redemption with a vast
                    northern portion containing the mountain resort town of
                    Strawberry. New Austin is an arid desert region on the
                    border with Mexico and centered on the frontier towns of
                    Armadillo and Tumbleweed, also featured in the original
                    game. Parts of New Austin and West Elizabeth have been
                    redesigned to reflect the earlier time; for example,
                    Blackwater is still under development, while Armadillo is a
                    ghost town as a result of a cholera outbreak.
                  </q-card-section>

                  <q-card-actions align="right">
                    <q-btn flat label="Close" color="black" v-close-popup />
                  </q-card-actions>
                </q-card>
              </q-dialog>
            </q-toolbar>
            <q-toolbar inset>
              <q-breadcrumbs active-color="black" style="font-size: 16px">
                <q-breadcrumbs-el label="Home" icon="home" />
                <q-breadcrumbs-el label="Components" icon="widgets" />
                <q-breadcrumbs-el label="Toolbar" />
              </q-breadcrumbs>
            </q-toolbar>
          </div>
        </div>
      </div>

      <template>
        <div class="q-px-lg q-pb-md text-white">
          <q-timeline color="red-10">
            <q-timeline-entry heading class="text-black text-center">
              Red Dead Redemption 2
              <br />
            </q-timeline-entry>

            <q-timeline-entry
              title="The Beginning"
              subtitle="January 22, 1899"
              side="left"
              icon="info"
            >
              <div class="text-weight-bolder">
                After a robbery goes badly wrong in the western town of
                Blackwater, Arthur Morgan and the Van der Linde gang are forced
                to flee. With federal agents and the best bounty hunters in the
                nation massing on their heels, the gang must rob, steal and
                fight their way across the rugged heartland of America in order
                to survive.
              </div>
            </q-timeline-entry>

            <q-timeline-entry
              title="Arthur Morgan"
              subtitle="Dutch's Second in command"
              side="right"
              icon="fa-solid fa-hat-cowboy-side"
            >
              <div class="text-weight-bolder">
                Arthur Morgan is a cold, brooding outlaw who often resorts to
                violence and has very few qualms about killing. At his worst
                Arthur could be extremely ruthless and completely unsympathetic
                to the people he hurts. Despite being capable of committing such
                violence, Arthur does have a playful side to his personality
                that comes out around those he is friendly with. He isnt above
                joking or employing sarcasm with his friends. Notably Arthur was
                kind and polite to John Marstons then-four-year-old son, Jack,
                having a gentle demeanor around the young boy in contrast to his
                threatening persona.
              </div>
            </q-timeline-entry>

            <q-timeline-entry heading class="text-red-10"
              >The Notorious Gang</q-timeline-entry
            >

            <q-timeline-entry
              title="The Van Der Line Gang"
              icon="fa-solid fa-skull-crossbones"
              subtitle="A gang of criminals, dissidents and free-thinkers who have chosen to reject a corrupt system of power and live instead by their own code."
              side="left"
            >
              <div class="text-weight-bolder">
                The Van der Linde gang, also referred to as Dutch's Boys is an
                outlaw gang featured in Red Dead Redemption 2 as the main
                protagonist faction. It is also mentioned in Red Dead
                Redemption, alongside the appearances of several of its former
                members.
              </div>
            </q-timeline-entry>

            <q-timeline-entry
              title="John Marston"
              icon="fa-solid fa-hat-cowboy-side"
              subtitle="People don't forget. Nothing gets forgiven."
              side="right"
            >
              <div class="text-weight-bolder">
                John has a strong dislike of birds and a rather dull
                imagination, especially when compared to his son Jack. When it
                comes to how he feels about religion, in-game quotes suggest
                that he is likely a Christian who is not overtly religious.
              </div>
            </q-timeline-entry>

            <q-timeline-entry
              title="The People"
              side="left"
              icon="fa-solid fa-person"
            >
              <div class="text-weight-bolder">
                Characters are the driving force behind the narrative of Red
                Dead Redemption 2 and include the various personalities and
                figures the player may and will encounter throughout their time
                in the game.
              </div>
            </q-timeline-entry>

            <q-timeline-entry
              title="RDR2 cumulative unit sales worldwide 2018-2022"
              side="right"
              icon="fa-solid fa-money-bill-1-wave"
            >
              <div class="text-weight-bolder">
                As of August 2022, Red Dead Redemption has sold 45 million units
                worldwide. The action-adventure game is developed by Rockstar
                games under the parent company Take-Two Interactive. First
                released in October 2018 for consoles, RDR2 had one of the
                biggest game launches of all time. However, these sales figures
                pale when compared to T2's biggest game in its vast portfolio:
                Grand Theft Auto 5, also developed by Rockstar Games, has sold
                approximately 170 million units since release.
              </div>
            </q-timeline-entry>

            <q-timeline-entry
              title="Metascore"
              subtitle="Red Dead Redemption 2 stands shoulder-to-shoulder with GTAV as one of the greatest games of the modern age"
              side="left"
              icon="fa-regular fa-star"
            >
              <div class="text-weight-bolder">
                Red Dead Redemption 2 won 4 awards, more than any other title,
                including Best Performance and Best Narrative.
              </div>
            </q-timeline-entry>
          </q-timeline>
        </div>
      </template>

      <div align="center">
        <q-img
          src="https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/d6a964da-f73f-431c-a95b-3d4477268790/ddhljyu-7ae3cfb8-17aa-48d1-b15b-d8717fb12903.png/v1/fill/w_1600,h_900,q_80,strp/red_dead_redemption_2___wallpaper_v_2_by_3demerzel_ddhljyu-fullview.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7ImhlaWdodCI6Ijw9OTAwIiwicGF0aCI6IlwvZlwvZDZhOTY0ZGEtZjczZi00MzFjLWE5NWItM2Q0NDc3MjY4NzkwXC9kZGhsanl1LTdhZTNjZmI4LTE3YWEtNDhkMS1iMTViLWQ4NzE3ZmIxMjkwMy5wbmciLCJ3aWR0aCI6Ijw9MTYwMCJ9XV0sImF1ZCI6WyJ1cm46c2VydmljZTppbWFnZS5vcGVyYXRpb25zIl19.KvQRIwLsMo5itgm0E24LBjF7-qoRFGVrRWYjD6XRwP4"
          style="max-width: 650px; height: 350px"
        >
          <div class="absolute-bottom text-subtitle1 text-center">
            <p>&copy; By Tizy. All Rights Reserved.</p>
          </div>
        </q-img>
      </div>

      <div class="q-mt-xl" align="center">
        <q-btn
          class="q-mt-xl"
          color="black"
          text-color="white"
          unelevated
          to="/"
          label="Logout"
          no-caps
          icon-right="code"
          position="bottom"
        />
      </div>
    </template>
  </q-page>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
    };
  },
};
</script>
