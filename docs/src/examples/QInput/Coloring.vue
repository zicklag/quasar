<template>
  <div class="q-pa-md">
    <div class="q-gutter-y-md column" style="max-width: 300px">
      <q-input color="purple-12" v-model="text" label="Label">
        <template v-slot:prepend>
          <q-icon name="event" />
        </template>
      </q-input>

      <q-input color="teal" filled v-model="text" label="Label">
        <template v-slot:prepend>
          <q-icon name="event" />
        </template>
      </q-input>

      <q-input color="lime-11" bg-color="green" filled v-model="text" label="Label">
        <template v-slot:prepend>
          <q-icon name="event" />
        </template>
      </q-input>

      <q-input color="teal" outlined v-model="text" label="Label">
        <template v-slot:append>
          <q-avatar>
            <img src="https://cdn.quasar-framework.org/img/quasar-logo.png">
          </q-avatar>
        </template>
      </q-input>

      <q-input color="orange" standout bottom-slots v-model="text" label="Label" counter>
        <template v-slot:prepend>
          <q-icon name="place" />
        </template>
        <template v-slot:append>
          <q-icon name="close" @click="text = ''" class="cursor-pointer" />
        </template>

        <template v-slot:hint>
          Field hint
        </template>
      </q-input>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      text: ''
    }
  }
}
</script>
