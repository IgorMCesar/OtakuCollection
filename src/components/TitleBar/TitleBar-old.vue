<template>
  <div>
    <el-col :span="8" class="app-name unselectable">
      Otaku Collection
    </el-col>
    <el-col ::xs="9" :sm="10" :md="11" :lg="12" :xl="13" class="buttons app-name">
      <user></user>
    </el-col>
    <el-col ::xs="7" :sm="6" :md="5" :lg="4" :xl="3" class="buttons">
      <Buttons></Buttons>
    </el-col>
  </div>
</template>

<script>
import User from '@/components/TitleBar/User';
import Buttons from '@/components/TitleBar/Buttons';

export default {
  components: { User, Buttons },
};
</script>

<style lang="scss" scoped>
.app-name {
  line-height: 40px;
}

.buttons {
  text-align: right;
}
</style>