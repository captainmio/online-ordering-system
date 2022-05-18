<template>
  <div class="row q-md full-height">
    <div class="col-7 ldiv">
      <!-- Login Card -->
      <card>
        <template v-slot:body>
          <q-form @submit="onSubmit" class="q-gutter-md">
            <textfield type="text" label="Email Address" v-model="email" />
            <textfield type="password" label="Password" v-model="password" />
            <div class="row pull-right">
              <btn type="submit" label="login" color="primary" />
            </div>
          </q-form>
        </template>
      </card>
    </div>
    <div class="col-5 rdiv">
      <img src="~assets/bg-login.svg" />
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
import card from "../components/Card.vue";
import textfield from "../components/InputTextfield.vue";
import btn from "../components/Button.vue";

export default {
  components: {
    card,
    textfield,
    btn,
  },
  setup() {
    const email = ref("");

    const onsubmit = () => {
      console.log(email);
    };

    return {
      email,
      onsubmit,
    };
  },
};
</script>

<style lang="scss" scoped>
.rdiv {
  background-color: #7992f7;
  height: 100vh;
  vertical-align: bottom;
  display: table-cell;
  position: relative;

  img {
    max-width: 100%;
    position: absolute;
    bottom: 0;
  }
}
</style>
