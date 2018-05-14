<template>
  <el-menu
      default-active="2"
      class="el-menu-vertical-demo"
      @open="handleOpen"
      @close="handleClose"
      background-color="#202326"
      text-color="#fff"
      active-text-color="#ffd04b">
      <el-submenu index="1">
        <template slot="title">
          <i class="el-icon-location"></i>
          <span>Navigator One</span>
        </template>
        <el-menu-item-group title="Group One">
          <el-menu-item index="1-1">item one</el-menu-item>
          <el-menu-item index="1-2">item one</el-menu-item>
          <el-menu-item index="1-3">item one</el-menu-item>
          <el-menu-item index="1-4">item one</el-menu-item>
          <el-menu-item index="1-5">item one</el-menu-item>
          <el-menu-item index="1-6">item one</el-menu-item>
          <el-menu-item index="1-7">item one</el-menu-item>
        </el-menu-item-group>
        <el-menu-item-group title="Group Two">
          <el-menu-item index="1-3">item three</el-menu-item>
        </el-menu-item-group>
        <el-submenu index="1-4">
          <template slot="title">item four</template>
          <el-menu-item index="1-4-1">item one</el-menu-item>
        </el-submenu>
      </el-submenu>
      <el-menu-item index="2">
        <i class="el-icon-menu"></i>
        <span>Navigator Two</span>
      </el-menu-item>
      <el-menu-item index="3" disabled>
        <i class="el-icon-document"></i>
        <span>Navigator Three</span>
      </el-menu-item>
      <el-menu-item index="4">
        <i class="el-icon-setting"></i>
        <span>Navigator Four</span>
      </el-menu-item>
    </el-menu>
</template>

<script>
  export default {
    data() {
      return {
        admins: [
          ['Management', 'people_outline'],
          ['Settings', 'settings'],
        ],
        cruds: [
          ['Create', 'add'],
          ['Read', 'insert_drive_file'],
          ['Update', 'update'],
          ['Delete', 'delete'],
        ],
      };
    },
    methods: {
      handleOpen(key, keyPath) {
        console.log(key, keyPath);
      },
      handleClose(key, keyPath) {
        console.log(key, keyPath);
      },
    },
  };
</script>

<style lang="scss" scoped>
.app-name {
  line-height: 40px;
}

.el-menu {
  border-right: 0px;
}

.el-button {
  background: #202326;
  color: white;
  border: 0px !important;
  border-radius: 0px;
  
  &:hover {
    background: white;
    color: #202326;
    border: 0px !important;
  }
}
.buttons {
  text-align: right;
}

.close:hover {
  background: #BF4F4E !important;
  color: white !important;
}
</style>