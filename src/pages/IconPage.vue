<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-back-button></ion-back-button>
        </ion-buttons>
        <ion-title>Icon组件演示</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
        Icon组件演示

        <ion-icon :icon="construct" class="red"></ion-icon>

      <br>
        <ion-icon :icon="peopleOutline"></ion-icon>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,  
  IonButtons,
  IonBackButton,
  IonIcon
} from "@ionic/vue";
import { construct,peopleOutline} from 'ionicons/icons';
export default {
  name: "IconPage",
  components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,    
    IonButtons,
    IonBackButton,
    IonIcon
  },
  setup(){
    return {
      construct,
      peopleOutline
    }
  }
};
</script>

<style scoped>
.red {
  font-size: 100px;
  color: red;
}
</style>