<template>
  <section class="wrap">
    <el-timeline>
      <el-timeline-item timestamp="版本 1.7.0" placement="top">
        <el-card>
          <h4>前端：</h4>
          <h4>升级 element-ui到2.15.5，更新部分npm包到最新版本</h4>
          <h4>新增 人事管理板块-员工管理、岗位管理和部门管理</h4>
          <h4>新增 数据字典管理：包含字典类型和字典数据视图</h4>
          <h4>新增 拖拽指令v-draggable和更改尺寸指令v-resizable，更改尺寸指令增加触发窗口change事件，触发组件重新布局</h4>
          <h4>新增 my-window窗口组件，支持dialog对话框和drawer抽屉自由切换。窗口支持页眉、页脚、代理窗口拖拽。更改尺寸支持8个方向拖拽。窗口拖拽边界和更改尺寸边界自动计算。抽屉窗口支持自动全屏展示。抽屉窗口支持上下左右4个方向拖拽更改尺寸。</h4>
          <h4>新增 岗位和部门选择组件</h4>
          <h4>新增 角色权限角色列表分页功能</h4>
          <h4>新增 视图同步信息_sync对象</h4>
          <h4>新增 视图同步功能，优化视图路径和视图命名</h4>
          <h4>新增 npm安装脚本</h4>
          <h4>新增 首页导航栏更改尺寸，文档管理分栏支持拖拽更改尺寸</h4>
          <h4>新增 个人设置已适应全屏展示，表单数据支持独立滚动</h4>
          <h4>调整 用户新增和修改下拉数据将从select数据中绑定，select数据直接同表单数据一并返回</h4>
          <h4>调整 将个性化分页和对话框组件移动到element-ui文件夹</h4>
          <h4>修改 my-markdown-editor组件使其支持@toast-ui/editor最新版本</h4>
          <h4>修改 所有界面弹出框统一使用my-window组件</h4>
          <h4>修改 权限管理删除接口操作，新增权限点可关联多接口</h4>
          <h4>修改 视图命名</h4>
          <h4>修改 空闲时间（分）最小值为0</h4>
          <h4>修复 请求路径使用query参数访问不断新增选项卡的问题</h4>
          <h4>修复 窗口表单下拉弹出层被遮挡的问题</h4>
          <h4>修复 分页禁用鼠标悬浮还高亮的问题</h4>
          <h4>删除 表格行索引</h4>
          <h4>优化 租户权限保存，设置权限保存时增加等待效果</h4>
          <h4>后端：</h4>
          <h4>更新 Nuget包到最新版本</h4>
          <h4>更新 数据包data.json</h4>
          <h4>新增 租户权限和字典类型模块</h4>
          <h4>新增 人事板块-员工、部门和岗位模块</h4>
          <h4>新增 租户权限、字典类型、员工、岗位和部门数据的导入和导出</h4>
          <h4>新增 基础仓储IRepositoryBase泛型注入，递归删除和递归软删除方法</h4>
          <h4>新增 租户管理设置权限功能，设置权限后同时删除租户关联的角色权限</h4>
          <h4>新增 权限点支持关联多接口功能</h4>
          <h4>新增 同步视图功能，优化视图路径和视图命名</h4>
          <h4>新增 基础服务BaseService通过属性懒加载获取获取实例的方法</h4>
          <h4>修改 数据字典重做，调整为数据字典类型和字典数据管理</h4>
          <h4>修改 IdleBus单例空闲时间回收设置逻辑</h4>
          <h4>修改 缓存键格式</h4>
          <h4>修复 token以旧换新异常的问题</h4>
          <h4>修复 非租户模式下导出数据包异常的问题</h4>
          <h4>修复 IpRateLimit更新最新版本异常的问题</h4>
          <h4>移除 角色权限仓储和用户角色仓储</h4>
          <h4>优化 租户设置权限限定租户权限范围，防止租户非法授权</h4>
          <h4>优化 雪花漂移算法新增是否启用判断</h4>
          <h4>优化 swagger api输入输出类同名无法加载的问题</h4>
          <p>小雪转中雪 提交于 2021-08-08</p>
        </el-card>
      </el-timeline-item>
      <el-timeline-item timestamp="版本 1.0.0" placement="top">
        <el-card>
          <h4>新增 更新日志</h4>
          <h4>新增 缓存管理，手动清除缓存</h4>
          <h4>修复 接口管理-同步Api异常问题</h4>
          <p>小雪转中雪 提交于 2020-3-24</p>
        </el-card>
      </el-timeline-item>
    </el-timeline>
    <el-backtop target=".container .main" :visibility-height="200" class="backtop" />
  </section>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
h2,h3,h4,h5 {
    font-weight: 400;
    color: #1f2f3d;
    margin-top: 0px;
    margin-bottom: 10px;
}
p {
    font-size: 14px;
    color: #5e6d82;
    line-height: 1.5em;
    margin-bottom: 0px;
}
.el-timeline{
  padding-left: 15px;
}

.wrap{
  padding:20px 80px 0px 8px;
}

@media screen and (max-width: 680px) {
  .wrap{
    padding:20px 10px 0px 8px;
  }

  .backtop {
    right: 5px !important;
    bottom: 5px !important;
  }
}
</style>
