<template>
    <div class="container">

        <br>

        <nav class="level">
            <div class="level-item has-text-centered">
                <div>
                    <p class="heading">SEARCH</p>
                    <b-field>
                        <b-input placeholder="Search..."
                                 type="search"
                                 icon="magnify">
                        </b-input>
                    </b-field>
                </div>
            </div>
            <div class="level-item has-text-centered">
                <div>
                    <p class="heading">FROM</p>
                    <b-datepicker
                            placeholder="Click to select..."
                            icon="calendar-today">
                    </b-datepicker>
                </div>
            </div>
            <div class="level-item has-text-centered">
                <div>
                    <p class="heading">To</p>
                    <b-datepicker
                            placeholder="Click to select..."
                            icon="calendar-today">
                    </b-datepicker>
                </div>
            </div>
        </nav>

        <br>
    </div>
</template>

<script>
  export default {
    name: 'Search',
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
