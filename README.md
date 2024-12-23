# 钉钉玲珑仓库（com.alibabainc.dingtalk.linyaps）

钉钉应用的玲珑项目文件

## 文件说明

| 名称                  | 必选        | 说明                                                                             |
| --------------------- | ----------- | -------------------------------------------------------------------------------- |
| deps.list             | 是          | 依赖包列表，忽略#开头注释                                                        |
| deps.all.list         | 自动生成    | 完整依赖列表                                                                     |
| deps.generated.list   | 自动生成    | 需要下载的依赖列表                                                               |
| sources.list          | 否,自动生成 | APT 源定义列表                                                                   |
| base.packages.list    | 否,自动生成 | 基础包环境包列表                                                                 |
| runtime.packages.list | 否,自动生成 | Runtime 包环境包列表                                                             |
| env.sh                | 否          | 构建前环境变量配置                                                               |
| build.sh              | 是          | 构建脚本入口                                                                     |
| install_dep.sh        | 是          | 依赖安装脚本                                                                     |
| install_patch.sh      | 否          | 补丁安装脚本                                                                     |
| install_start.sh      | 是          | 程序入口生成脚本                                                                 |
| patch\_\*.sh          | 否          | 补丁脚本                                                                         |


## 补丁列表

* patch_ld.sh: LD_LIBRARY_PATH 补丁
* patch_icon.sh: desktop图标补丁
* patch_gtk3-im.sh： gtk3输入法模块补丁