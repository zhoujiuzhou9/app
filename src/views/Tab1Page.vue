<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Tab 1</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-button router-link="/button"> 跳转到Button </ion-button>
      <ion-button @click="this.$router.push('/icon')"> 跳转到Icon </ion-button>
      <ion-button router-link="/toolbar"> 跳转到toolbar </ion-button>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
  IonButton,
} from "@ionic/vue";
</script>
