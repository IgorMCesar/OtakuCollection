<template>
  <el-tabs type="border-card">
    <el-tab-pane label="Watching">
      <el-table :data="tableData3" border style="width: 100%" height="calc(100% - 38px)">
        <el-table-column fixed prop="date" label="Date" width="150">
        </el-table-column>
        <el-table-column prop="name" label="Name" width="120">
        </el-table-column>
        <el-table-column prop="state" label="State" width="120">
        </el-table-column>
        <el-table-column prop="city" label="City" width="120">
        </el-table-column>
        <el-table-column prop="address" label="Address" width="300">
        </el-table-column>
        <el-table-column prop="zip" label="Zip" width="120">
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

  .el-tabs {
    border: 10px;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
    height:100% !important;
    width:100% !important;
  }
  
  .el-tab-pane {
    height:100% !important;
    width:100% !important;
  }

.el-table--border::after{
  position: relative;
}
</style>

<style>
  .el-tabs__content{
    height: 100% !important;
    padding: 10px 0px 0px 0px !important;
  }

  .el-tabs__nav-scroll,
  .el-tabs__header {
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
  }
</style>
