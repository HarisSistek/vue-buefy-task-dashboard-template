<template>
    <div class="container">
        <b-tabs type="is-boxed" v-model="activeTab">
            <b-tab-item>
                <template slot="header">
                    <b-icon icon="file-tree" />
                    <span> Tasks </span>
                </template>
                <TaskTab></TaskTab>
            </b-tab-item>
            <b-tab-item>
                <template slot="header">
                    <b-icon icon="chart-line" />
                    <span> Stats </span>
                </template>
                <StatsTab></StatsTab>
            </b-tab-item>
        </b-tabs>
    </div>
</template>

<script>
    import TaskTab from './Tabs/TaskTab';
    import StatsTab from './Tabs/StatsTab';
    export default {
        name: 'TaskTabs',
        components: {TaskTab, StatsTab},
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
