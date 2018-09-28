<template>
<q-layout>
  <q-layout-header>
    <q-toolbar :inverted="$q.theme === 'ios'" color='dark'>
      <q-toolbar-title>
        Bvoting
      </q-toolbar-title>
      <q-btn flat dense icon="add"  @click="addPoll()" aria-label="Add new vote" />
    </q-toolbar>
    <!-- header content -->
  </q-layout-header>
  <q-page-container>
    <q-page>
      <div class="q-pa-sm row justify-center">
        <q-card padding inline style="width: 300px;">
          <q-card-title>
            How do you like Bvoting?
          </q-card-title>
          <q-card-separator />
          <q-card-actions>
            <q-btn flat color="primary" label="Vote"/>
          </q-card-actions>
        </q-card>
      </div>
      <q-modal v-model="false">
        <h4>Basic Modal</h4>
      </q-modal>
    </q-page>
  </q-page-container>
</q-layout>
</template>

<script>
export default {
  name: 'MyLayout',
  data () {
    return {
      a: 10
    }
  },
  methods: {
    addPoll: function () {
      console.log('"Hello"')
    }
  }
}
</script>

<style>
</style>
