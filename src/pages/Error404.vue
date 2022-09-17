<template>
  <div
    class="fullscreen bg-accent text-black text-center q-pa-md flex flex-center"
  >
    <div>
      <div style="font-size: 30vh">404</div>

      <div class="text-h2" style="opacity: 0.4">
        Oops. Nothing here partner ...
      </div>

      <q-btn
        class="q-mt-xl"
        color="red-10"
        text-color="black"
        unelevated
        to="/"
        label="Go Home, you're drunk"
        no-caps
        icon-right="send"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "ErrorNotFound",
};
</script>
