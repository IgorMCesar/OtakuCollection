<template>
  <div class="no-drag border ue">
    <el-container>
        <el-header class="drag header">
            <titlebar></titlebar>
        </el-header>
        <el-container>
            <el-aside class="sidenav-component">
              <SideNavMenu></SideNavMenu>
            </el-aside>
          <el-container>
              <el-main>Main</el-main>
            <el-footer>Footer</el-footer>
          </el-container>
        </el-container>
    </el-container>
  </div>
</template>


<script>
  import Titlebar from '@/components/TitleBar/TitleBar';
  import SideNavMenu from '@/components/SideNavMenu/SideNavMenu';

  export default {
    name: 'index',
    components: { Titlebar, SideNavMenu },
  };
</script>

<style lang="scss">

// .header {
//   top: 0;
//   overflow: hidden;
//   width: 100%;
//   position: fixed;
//   z-index: 101;
// }

.el-footer {
  position: fixed;
  bottom: 0px;
  width: 100%;
  //max-height: calc(100% - 100px);
  height: 20px !important;
  left: 280px;
  max-width: calc(100% - 280px);
  background-color: #202326;
}

.el-main {
  position: fixed;
  top: 40px;
  max-height: calc(100% - 100px);
  left: 280px;
  max-width: calc(100% - 280px);
}

.sidenav-component {
  height: 100%;
  width: 280px !important;
  overflow-y: auto;
  position: absolute;
  background-color:#202326;
}

.el-header {
  background-color: #202326;
  color: rgb(255, 255, 255);
  line-height: 30px;
  height: 40px !important;
  padding: 0px 0px 0px 20px;
}

.el-aside {
  color: #333;
  top: 40px;
  max-height: calc(100% - 40px);
}
</style>