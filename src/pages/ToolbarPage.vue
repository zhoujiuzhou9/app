<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-back-button></ion-back-button>
        </ion-buttons>
        <ion-title>ToolbarPage</ion-title>
        <ion-buttons slot="end">
          <ion-button fill="clear" color="dark">
            <ion-icon slot="icon-only" :icon="grid"></ion-icon>
          </ion-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-header>
    <ion-content> ToolbarPage </ion-content>
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
  //   IonIcon
} from "@ionic/vue";
import { grid } from "ionicons/icons";
export default {
  name: "ToolbarPage",
  components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,
    IonButtons,
    IonBackButton,
    // IonIcon
  },
  setup() {
    return {
      grid,
    };
  },
};
</script>
