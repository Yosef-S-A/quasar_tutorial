<template>
  <q-page padding>
    <!-- <q-card style="width: 350px">
      <q-card-section class="bg-blue text-white"> My Card </q-card-section>
      <q-card-section>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit, cum! Vel
        velit ipsum distinctio odio exercitationem assumenda est itaque, animi
        possimus inventore harum quam unde consequuntur quidem temporibus
        corporis incidunt.
      </q-card-section>
    </q-card> -->
    <q-select
      v-model="selected"
      label="beings"
      :options="['Luke', 'Yosef', 'Dawit']"
    >
    </q-select>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",

  data() {
    return {
      selected: null,
    };
  },
});
</script>
