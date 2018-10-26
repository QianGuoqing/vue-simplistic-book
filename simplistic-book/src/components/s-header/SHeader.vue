<template>
  <div class="header-wrapper">
    <Row>
      <Col span="3">
        <div class="logo"></div>
      </Col>
      <Col span="16">
        <nav>
          <div class="menu">
            <div class="index-page">首页</div>
            <div class="download-app">下载App</div>
            <Input suffix="ios-search" placeholder="搜索" style="width: auto" />
          </div>
          <div class="aa-login">
            <div class="aa">Aa</div>
            <div class="login">登陆</div>
          </div>
        </nav>
      </Col>
      <Col span="5">
        <div class="write-register">
          <div class="register">注册</div>
          <div class="write">
            <Icon type="md-create" />写文章
          </div>
        </div>
      </Col>
    </Row>
  </div>
</template>

<script>
  export default {
    name: 'SHeader'
  }
</script>

<style lang="stylus" scoped>
  .header-wrapper
    height 56px
    border-bottom 1px solid #f0f0f0
    position relative
    z-index 1
    .logo
      display block
      width 100px
      height 56px
      background url('../../../static/logo.png')
      background-size contain
      cursor pointer
    nav
      display flex
      justify-content space-between
      align-items center
      height 56px
      font-size 17px
      .menu
        display flex
        align-items center
        .index-page
          color #ea6f5a
          cursor pointer
          margin-right 20px
          font-weight bolder
        .download-app
          color #333
          margin-right 20px
          cursor pointer
      .aa-login
        display flex
        align-items center
        padding-right 25px
        color #969696
        font-size 17px
        font-weight bolder
        .aa
          margin-right 30px
          cursor pointer
        .login
          cursor pointer
    .write-register
      height 56px
      display flex
      align-items center
      font-weight bolder
      .register
        border 1px solid #ec6149
        color #ec6149
        padding 10px 20px
        border-radius 20px
        font-size 14px
        margin-right 20px
        cursor pointer
      .write
        border 1px solid #ec6149
        background-color #ec6149
        color #fff
        padding 10px 20px
        border-radius 20px
        font-size 14px
        cursor pointer
</style>