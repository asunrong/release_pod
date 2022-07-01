fastlane documentation
----

# Installation

Make sure you have the latest version of the Xcode command line tools installed:

```sh
xcode-select --install
```

For _fastlane_ installation instructions, see [Installing _fastlane_](https://docs.fastlane.tools/#installing-fastlane)

# Available Actions

### release_pod

```sh
[bundle exec] fastlane release_pod
```


## Quick Use

1. cd your pod_project_root_patch (在你项目的根目录下)
2. vim fastlane/Fastfile  add this codes to your Fastfile (在你的fastlane/Fastfile 中添加如下代码)

```Ruby
 import_from_git(url: 'https://github.com/asunrong/release_pod.git')

 desc "Noew you can and your CI"
 lane :new_main_lane do
 UI.message("🎉you can and your CI 🎉")
 end
```

3. Option copy  autoPodRelease.sh your_project ./fastlane/Script/autoPodRelease.sh (复制本项目中的autoPodRelease.sh 内容到你工程./fastlane/Script/autoPodRelease.sh 中)


### Quick start (快速启动,执行autoPodRelease.sh 版本号 )

```sh
 # 改完代码后,一键pod脚本,只有一个必须参数,即只需指定版本即可.例如0.1.2 (自动打tag 并pod 发布
 autoPodRelease.sh 0.1.2
```

release_pod 航道用来自动化升级维护pod库


----

This README.md is auto-generated and will be re-generated every time [_fastlane_](https://fastlane.tools) is run.

More information about _fastlane_ can be found on [fastlane.tools](https://fastlane.tools).

The documentation of _fastlane_ can be found on [docs.fastlane.tools](https://docs.fastlane.tools).
