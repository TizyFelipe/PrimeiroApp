<template>
  <q-page
    style="
      background-image: url('https://i.pinimg.com/originals/9b/1b/9a/9b1b9ad001dd99b612147a431d668023.png');
      background-size: cover;
    "
    class="flex flex-center"
  >
    <div>
      <div style="width: 300px">
        <q-input
          color="black"
          v-model="usuario"
          outlined
          type="text"
          label="User"
          class="bg-accent"
        >
          <template v-slot:append>
            <q-avatar>
              <img
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ_pf4Gi2YBpL0VTU1wFU61aZrpCcMkcZ22JXldxBMjJLqtM341E6-mI1h-_9M2_cQh8-c&usqp=CAU"
              />
            </q-avatar>
          </template>
        </q-input>
        <q-input
          color="black"
          v-model="senha"
          outlined
          type="password"
          label="Password"
          class="bg-accent"
        />
      </div>
      <div class="q-mt-sm" align="center">
        <q-btn
          push
          color="red-10"
          text-color="dark"
          label="Login"
          icon-right="send"
          to="/primeira"
        />

        <q-btn
          push
          color="red-10"
          text-color="dark"
          label="Howdy, i'm new!"
          icon-right="warning"
          to="/formulario"
        />
      </div>
    </div>
    <div class="absolute-bottom text-subtitle1 text-center">
      <p>&copy; By Tizy. All Rights Reserved.</p>
    </div>
  </q-page>
</template>

<script>
export default {
  // name: "PageIndex",
  // data() {
  //   return {
  //     usuario: "",
  //     senha: "",
  //   };
  // },
  // methods: {
  //   login() {
  //     const dados = {
  //       usuario: this.usuario,
  //       senha: this.senha,
  //     };
  //     console.log(dados);
  //     this.$axios.post("http://localhost:5000/login", dados);
  //   },
  // },
};
</script>

<style scoped>
.bg_image {
  background: cover;
}
</style>

//class="flex flex-center">
