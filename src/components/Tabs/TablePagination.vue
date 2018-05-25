<template>
    <section>
        <hr>
        <b-field grouped group-multiline>
            <b-field label="Total">
                <b-input type="number" v-model="total"></b-input>
            </b-field>
            <b-field label="Items per page">
                <b-input type="number" v-model="perPage"></b-input>
            </b-field>
        </b-field>

        <b-pagination
                :total="total"
                :current.sync="current"
                :order="order"
                :size="size"
                :simple="isSimple"
                :rounded="isRounded"
                :per-page="perPage">
        </b-pagination>
    </section>
</template>

<script>
  export default {
    data() {
      return {
        total: 200,
        current: 1,
        perPage: 20,
        order: 'is-centered',
        size: 'is-small',
        isSimple: false,
        isRounded: false
      }
    }
  }
</script>