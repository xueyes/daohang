<template>
  <div class="index">
      <!-- 侧边栏 -->
      <div class="side-menu">
          <h2 class="side-menu__tt">极客猿梦导航</h2>

          <ul class="side-menu__list">
              <li v-for="item in menuList" class="side-menu__item">{{item}}</li>
          </ul>
      </div>
  </div>

</template>

<script>
export default {
    name: 'index',
    data: function() {
        return {
            menuList: ['网络运营', '设计素材', '实用工具', '技术博客', '开发社区']
        }
    }
}
</script>



<style lang="scss" scoped>


.index,
.side-menu {
    height: 100%;
}
.side-menu {
    position: fixed;
    background: #30333c;
    color: #6b7386;
    box-sizing: border-box;
    flex-direction: column;
    display: flex;
    width: 248px;
    transition: all .5s;
}
.side-menu__tt {
    color: #fff;
    text-align: center;
    font-weight: 500;
    padding-bottom: 20px;
    border-bottom: 2px solid rgba(255,255,255,.04);
}
.side-menu__list {

}
.side-menu__item {
    padding: 15px 0;
}
</style>



