<template>
  <div>
        <el-container>
          <el-header style="text-align: right; font-size: 12px">
            <p style="position:fixed;top:-15px;left:20px;font-size:24px;">猴戏网</p>
              <el-dropdown>
                <i class="el-icon-setting" style="margin-right: 15px"></i>
                <el-dropdown-menu slot="dropdown">
                  <el-dropdown-item>查看</el-dropdown-item>
                  <el-dropdown-item>新增</el-dropdown-item>
                  <el-dropdown-item>删除</el-dropdown-item>
                </el-dropdown-menu>
              </el-dropdown>
              <span> 您好 猴戏</span>&nbsp;&nbsp;&nbsp;
              <span style="display:inline-block; margin-left:10px;">退出登录</span>
            </el-header>
        

        <el-submenu index="1">
                <template slot="title"><i class="el-icon-setting"></i>设置</template>
              </el-submenu>
        <el-container style="height: 500px; border: 1px solid #eee">
          <el-aside width="200px" >
            <!-- style="background-color: rgb(238, 241, 246)" -->
            <el-menu :default-openeds="['1']">
              <el-submenu index="1">
                <template slot="title"><i class="el-icon-setting"></i>工作前台</template>
              </el-submenu>
              <el-submenu index="2">
                <template slot="title"><i class="el-icon-message"></i>咨询</template>
                <el-menu-item-group>
                  
                  <el-menu-item index="1-1">车与出行</el-menu-item>
                  <el-menu-item index="1-2">年轻一代</el-menu-item>
                  <el-menu-item index="1-3">十亿消费者</el-menu-item>
                  <el-menu-item index="1-4">前沿科技</el-menu-item>
                  <el-menu-item index="1-15">财经</el-menu-item>
                  <el-menu-item index="1-5">娱乐淘金</el-menu-item>
                  <el-menu-item index="1-6">医疗健康</el-menu-item>
                  <el-menu-item index="1-7">文化教育</el-menu-item>
                  <el-menu-item index="1-8">出海</el-menu-item>
                  <el-menu-item index="1-9">金融地产</el-menu-item>
                  <el-menu-item index="1-10">企业服务</el-menu-item>
                  <el-menu-item index="1-11">创业维艰</el-menu-item>
                  <el-menu-item index="1-12">社交通讯</el-menu-item>
                  <el-menu-item index="1-13">全球热点</el-menu-item>
                  <el-menu-item index="1-14">生活腔调</el-menu-item>
                </el-menu-item-group>
             
              </el-submenu>
              <el-submenu index="3">
                <template slot="title"><i class="el-icon-menu"></i>视频</template>
              
              </el-submenu>
              <el-submenu index="4">
                <template slot="title"><i class="el-icon-setting"></i>24小时</template>
              </el-submenu>

              <el-submenu index="5">
                <template slot="title"><i class="el-icon-setting"></i>用户管理</template>
              </el-submenu>

              
            </el-menu>
          </el-aside>
          
          <el-container>
            
            
            <el-main>
              <el-table :data="tableData">
                <el-table-column prop="date" label="日期" width="140">
                </el-table-column>
                <el-table-column prop="name" label="姓名" width="120">
                </el-table-column>
                <el-table-column prop="address" label="地址">
                </el-table-column>
              </el-table>
            </el-main>
          </el-container>
        </el-container>
      </el-container>
  </div>
</template>

<script>
export default {
     data() {
      const item = {
        date: '2016-05-02',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1518 弄'
      };
      return {
        tableData: Array(20).fill(item)
      }
    }
}
</script>

<style scoped>
.el-header {
    background-color: #B3C0D1;
    color: #333;
    line-height: 60px;
  }
  
  .el-aside {
    color: #333;
  }
</style>