<template>
  <div id="app">
     <button id="jest" @click="onClose" />
    <button id="modalbtn" @click="showModal = true" class="button" outlined>Abone Ol</button>
    <a v-if="isLoggedin" id="profile">my profile</a>
    <transition name="fade" appear>
      <div
        class="modal-overlay"
        v-if="showModal"
        @click="showModal = false"
      ></div>
    </transition>
    <transition name="slide" appear>
      <div class="modal" role="dialog" v-if="showModal">
        <v-container>
          <v-row>
            <v-col>
              <v-img
                max-height="600px"
                max-width="500px"
                src="https://www.camper.com/img/BLF.webp?d=20211212"
                class="ml-auto"
              ></v-img>
            </v-col>
            <v-col>
              <v-card class="pa-2" outlined tile>
                <h1>Kaydolun ve %10 İndirim Kazanın</h1>
                <p>
                  Camper Ailesi'nin bir parçası olmak size özel promosyonlara ve
                  hikayelere erişim sağlayacaktır.
                </p>
                <v-text-field
                  label="E-mail adresinizi girin"
                  outlined
                ></v-text-field> </v-card
            ></v-col>
          </v-row>
         
          <button id="abonBtn" @click="showModal = false" class="button">
            Abone Ol
          </button>
        </v-container>
      </div>
    </transition>
  </div>
</template>

<style lang="scss">
body {
  font-family: "montserrat", sans-serif;
}
#app {
  height: auto;
  width: 200px;
  overflow: hidden;
}

.button {
  appearance: none;
  border-style: solid;
  border-radius: unset;
  background: none;
  cursor: pointer;
  margin-top: 10px;
  display: inline-block;
  padding: 12px 22px;
  color: #222;
  font-weight: 500;
  transition: 0.4s;
  &:hover {
    background-color: black;
    color: white;
  }
}

#abonBtn {
  margin-left: 120px;
}
.modal-overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 98;
  background-color: rgba(0, 0, 0, 0.2);
}

.modal {
  position: absolute;
  top: 50%;
  left: 50%;
  z-index: 99;

  width: 100%;
  max-width: 414px;
  transform: translate(-50%, -50%);

  background-color: #fff;
  border-radius: 16px;

  padding: 25px;

  h1 {
    color: #222;
    font-size: 32px;
    font-weight: 300;
    margin-bottom: 15px;
  }

  p {
    color: #666;
    font-size: 18px;
    font-weight: 400;
    margin-bottom: 15px;
  }
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter,
.fade-leave-to {
  opacity: 0;
}

.slide-enter-active,
.slide-leave-active {
  transition: transform 0.5s;
}
.slide-enter,
.slide-leave-to {
  transform: translateY(-50%) translateX(100vw);
}
</style>
<script>
export default {
  props: ["onClose"],
  data() {
    return {
      isLoggedin: false,
      showModal: false,
    };
  },
};
</script>