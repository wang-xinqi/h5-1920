# git
    + 分布式版本控制工具

# git 工作流程
    + 工作区（写代码的终端）
    + 暂存区
    + 版本库
    `txt
        工作的流程：
            1：工作区写代码
            2：工作区代码编辑完毕，将代码提交到暂存区
                - 暂存区：类似于过滤层，保护工作区与版本库的代码， 避免错误操作。
            3：将暂存区的代码 提交到 版本库，形成版本（版本可以进行处理）
    `
    + 将版本库内容迁到远端（github\gitee）


# 下载git


# 在 git bash 终端操作 查看git版本

    + $ git --version
        -git version 2.23.0.windows.1


# git 第一次操作需要配置个人信息

    + $ git config --global user.name 名字
    + $ git config --global user.email 邮箱地址
    + $ git config --list 查看配置信息


# 一项目（工作区）被git管理 先初始化git

    + $ git init    当前项目被git管理
        - git默认情况下不会管理空文件
        - git管理文件包括所有的子文件



# 查看当前被git管理的项目文件的状态
    + $ git status  
        - 如果文件显示红色：文件在工作区没有向暂存区提交
        - 如果文件显示绿色：文件在暂存区没有向版本库提交

# 将工作区的文件提交到暂存区
    + $ git add index.html   提交某个文件
    + $ git add css/         提交某个文件夹
    + $ git add --all        提交所有
    + $ git add .            提交所有


# 将暂存区的文件拉回到工作区
    + $ git reset HEAD -- index.html    拉回某个文件
    + $ git reset HEAD -- css/          拉回某个文件夹
    + $ git reset HEAD -- .           拉回所有