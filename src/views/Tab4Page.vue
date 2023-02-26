<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Tab 4</ion-title>
        <ion-buttons slot="end">
          <ion-button fill="clear" color="dark">
            <ion-icon slot="icon-only" :icon="grid"></ion-icon>
          </ion-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      Tab 4
      <ion-button>
        按钮
      </ion-button>
      <ion-icon :icon="grid"></ion-icon>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent,IonButton,IonIcon } from '@ionic/vue';
import {grid,add} from 'ionicons/icons';
</script>
