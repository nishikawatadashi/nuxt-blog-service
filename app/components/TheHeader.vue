<template>
  <el-menu
    :router="true"
    mode="horizontal">
    <el-menu-item
      index="1"
      style="pointer-events:none;">
      Nuxt Diary App
    </el-menu-item>
    <el-menu-item
      :router="{ path: '/posts/' }"
      index="2">
      投稿一覧
    </el-menu-item>

    <no-ssr>
      <el-menu-item
        :router="{ path: '/' }"
        index="4"
        style="float: right;">
        <span>ログイン</span>
      </el-menu-item>
    </no-ssr>
    <el-menu-item
      :router="{ path: '/posts/new' }"
      index="5"
      style="float: right;">
      新規投稿
    </el-menu-item>
  </el-menu>
</template>
