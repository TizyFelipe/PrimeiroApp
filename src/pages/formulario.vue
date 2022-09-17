<template>
  <q-page class="flex flex-center bg-grey-10">
    <div class="q-pa-md" style="max-width: 400px">
      <q-card class="my-card bg-grey-7">
        <q-card-section>
          <q-form @submit="onSubmit" @reset="onReset" class="q-gutter-md">
            <q-input
              standout="bg-grey-7 text-white"
              dense
              filled
              v-model="name"
              label="Your name *"
              hint="Name and surname"
              lazy-rules
              :rules="[(val) => val.length > 0 || 'Type your name']"
            />

            <q-input
              standout="bg-grey-7 text-white"
              dense
              filled
              v-model="name"
              label="New Login *"
              hint="login"
              lazy-rules
              :rules="[(val) => (val && val.length > 0) || 'Create a Login']"
            />

            <q-input
              standout="bg-grey-7 text-white"
              dense
              filled
              type="number"
              v-model="age"
              label="Your age *"
              lazy-rules
              :rules="[
                (val) => (val !== null && val !== '') || 'Type your age',
                (val) => (val >= 5 && val <= 99) || 'Type a real age',
              ]"
            />

            <q-input
              standout="bg-grey-7 text-white"
              dense
              filled
              type="text"
              v-model="phone"
              label="Phone Number *"
              lazy-rules
              mask="(##) #####-####"
              :rules="[(val) => val.length == 15 || 'Type your phone ']"
            />

            <q-toggle v-model="accept" label="I accept all the terms" />

            <div class="row justify-center">
              <q-btn
                label="Submit"
                type="submit"
                color="red-10"
                text-color="black"
                :disable="!accept"
              />
              <q-btn
                label="Clear"
                type="reset"
                color="red-10"
                text-color="black"
                class="q-ml-sm"
              />
            </div>

            <div class="q-mt-xl" align="center">
              <q-btn
                class="q-mt-xl"
                color="red-10"
                text-color="black"
                unelevated
                to="/"
                label="Go Back"
                no-caps
                icon="directions"
                position="bottom"
              />
            </div>
          </q-form>
        </q-card-section>
      </q-card>
    </div>
  </q-page>
</template>

<script>
export default {
  data() {
    return {
      name: null,
      age: null,
      adress: null,
      phone: null,
      accept: false,
    };
  },

  methods: {
    onSubmit() {
      if (this.accept !== true) {
        this.$q.notify({
          color: "red-5",
          textColor: "white",
          icon: "warning",
          message: "You need to accept the license and terms first",
        });
      } else {
        this.$q.notify({
          color: "green-4",
          textColor: "white",
          icon: "cloud_done",
          message: "Submitted",
        });
      }
    },

    onReset() {
      this.name = null;
      this.age = null;
      this.adress = null;
      this.phone = null;
      this.accept = false;
    },
  },
};
</script>
