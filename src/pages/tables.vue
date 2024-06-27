<script setup>
import InfoCard from "@/components/cards/InfoCard.vue";
import { VCol, VRow } from "vuetify/lib/components/index.mjs";
</script>
<template>
  <VCard>
    <VCardItem>
      <VCardTitle>โต๊ะในร้าน</VCardTitle>
    </VCardItem>
    <VCardText>
      <VRow>
        <VCol cols="3">
          <InfoCard
            title="โต๊ะทั้งหมด"
            :stats="10"
            unit="ตัว"
            icon="mdi-table"
            color="primary"
          />
        </VCol>
        <VCol cols="3">
          <InfoCard
            title="โต๊ะว่าง"
            :stats="5"
            unit="ตัว"
            icon="mdi-table-plus"
            color="success"
          />
        </VCol>
        <VCol cols="3">
          <InfoCard
            title="ใช้งานอยู่"
            :stats="5"
            unit="ตัว"
            icon="mdi-table-account"
            color="warning"
          />
        </VCol>
        <VCol cols="3">
          <VCard class="align-center justify-center d-flex fill-height">
            <VBtn                
              class="fill-height"
              variant="text"
              block
              text
            >
              <VIcon>mdi-plus</VIcon>
              เพิมโต๊ะใหม่
            </VBtn>
          </VCard>
        </VCol>
      </VRow>
    </VCardText>
  </VCard>
  <VCard class="mt-8">
    <VCardText>
      <VRow>
        <VCol cols="3"><v-btn size ="300" color="green">โต๊ะที่1</v-btn></VCol>
        <VCol cols="3"><v-btn size ="300" color="green">โต๊ะที่2</v-btn></VCol>
        <VCol cols="3"><v-btn size ="300" >โต๊ะที่3</v-btn></VCol>
        <VCol cols="3"><v-btn size ="300">โต๊ะที่4</v-btn></VCol>
    </VRow>
    <VRow>
        <VCol cols="3"><v-btn size ="300" color="green">โต๊ะที่5</v-btn></VCol>
        <VCol cols="3"><v-btn size ="300" color="green">โต๊ะที่6</v-btn></VCol>
        <VCol cols="3"><v-btn size ="300" color="green">โต๊ะที่7</v-btn></VCol>
        <VCol cols="3"><v-btn size ="300">โต๊ะที่8</v-btn></VCol>
    </VRow>
    <VRow>
        <VCol cols="3"><v-btn size ="300" >โต๊ะที่9</v-btn></VCol>
        <VCol cols="3"><v-btn size ="300">โต๊ะที่10</v-btn></VCol>

    </VRow>
    </VCardText>
  </VCard>
</template>
