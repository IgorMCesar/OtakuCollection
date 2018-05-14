<template>
  <el-tabs type="border-card" class="full">
    <el-tab-pane label="Watching">
      <el-table
        :data="tableData3"
        style="width: 100%"
        height="100%"
        fixed
        >
        <el-table-column
          prop="date"
          label="Date"
          width="150">
        </el-table-column>
        <el-table-column
          prop="name"
          label="Name"
          width="120">
        </el-table-column>
        <el-table-column
          prop="state"
          label="State"
          width="120">
        </el-table-column>
        <el-table-column
          prop="city"
          label="City"
          width="120">
        </el-table-column>
        <el-table-column
          prop="address"
          label="Address"
          width="300">
        </el-table-column>
        <el-table-column
          prop="zip"
          label="Zip"
          width="120">
        </el-table-column>
      </el-table>
    </el-tab-pane>
    <el-tab-pane label="Completed">Config</el-tab-pane>
    <el-tab-pane label="On hold">Role</el-tab-pane>
    <el-tab-pane label="Dropped">Task</el-tab-pane>
    <el-tab-pane label="Plan to watch">Task</el-tab-pane>
  </el-tabs>
</template>

<script>
  export default {
    data() {
      return {
        tableData3: [{
          date: '2016-05-03',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-02',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-04',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-01',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-08',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-06',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-06',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-06',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-06',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-06',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }, {
          date: '2016-05-07',
          name: 'Tom',
          state: 'California',
          city: 'Los Angeles',
          address: 'No. 189, Grove St, Los Angeles',
          zip: 'CA 90036',
        }],
      };
    },
  };
</script>

<style lang="scss" scoped>

  .full {
    height: 100%;
    max-height: 100%;
  }

  .fixed-stuff {
    position: fixed;
    transition: none;
    max-width: 100%;
    overflow: scroll;
    will-change: transform;
  }

</style>

