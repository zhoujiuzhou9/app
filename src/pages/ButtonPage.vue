<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-back-button></ion-back-button>
        </ion-buttons>
        <ion-title>button按钮组件演示andre</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
      <ion-button> 普通按钮 </ion-button>
      <ion-button color="success"> Click me </ion-button>

      <ion-button expand="full"> Click me full </ion-button>

      <ion-button expand="block"> Click me block </ion-button>

      <ion-button fill="clear"> Click me clear </ion-button>

      <ion-button fill="outline"> Click me outline </ion-button>
      <ion-button fill="solid" color="dark"> Click me solid </ion-button>

      <ion-button size="small" color="dark"> Click me small </ion-button>

      <ion-button mode="ios" color="primary"> ios 平台的按钮 </ion-button>
      <ion-button mode="md" color="primary">android 平台的按钮 </ion-button>


      <ion-button color="primary">
          <ion-icon slot="start" :icon="person"></ion-icon>
          用户
      </ion-button>
     
      <ion-button color="primary">        
          收藏
           <ion-icon slot="end" :icon="star"></ion-icon>
      </ion-button>

      <ion-button fill="clear" color="dark">
          <ion-icon slot="icon-only" :icon="star"></ion-icon>
         
      </ion-button>

      <ion-icon :icon="star"></ion-icon>

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
  IonButton,
  IonButtons,
  IonBackButton,
  IonIcon
} from "@ionic/vue";

import { person,star} from 'ionicons/icons';

export default {
  name: "ButtonPage",
  components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,
    IonButton,
    IonButtons,
    IonBackButton,
    IonIcon
  },setup(){
    return{
      person,
      star
    }
  }
};
</script>
