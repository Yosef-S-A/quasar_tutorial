<template>
  <q-page class="row">
    <!-- <q-card style="width: 350px">
      <q-card-section class="bg-blue text-white"> My Card </q-card-section>
      <q-card-section>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit, cum! Vel
        velit ipsum distinctio odio exercitationem assumenda est itaque, animi
        possimus inventore harum quam unde consequuntur quidem temporibus
        corporis incidunt.
      </q-card-section>
    </q-card> -->
    <!-- <q-select
      v-model="selected"
      label="beings"
      :options="['Luke', 'Yosef', 'Dawit']"
    >
    </q-select> -->

    <q-card class="col-xs-9">
      <q-toolbar>
        <q-input
          :model-value="search"
          class="full-width"
          borderless
          dense
          placeholder="Search"
        >
          <template #append>
            <q-icon name="mdi-magnify"></q-icon>
          </template>
        </q-input>
      </q-toolbar>
      <q-list bordered>
        <q-item>
          <q-item-section side>
            <q-checkbox :model-value="true"></q-checkbox>
          </q-item-section>
          <q-item-section> Go Shopping </q-item-section>
          <q-item-section side>
            <q-btn flat round icon="mdi-delete"></q-btn>
          </q-item-section>
        </q-item>
      </q-list>
    </q-card>
    <div class="col-xs-3">
      <q-toolbar class="bg-primary">
        <q-btn
          fab
          color="secondary"
          icon="mdi-plus"
          style="margin-bottom: -42px"
          class="q-ml-md"
        ></q-btn>
      </q-toolbar>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",

  data() {
    return {
      search: "",
    };
  },
});
</script>
