# DetailsOnWindowsUsage
## 报错&amp;警告&amp;心得体会-原因分析&amp;解决办法&amp;经验总结
## 长期更新, 当前时间是2019年6月15日10:11:36

- 操作无法完成因为文件已在{?}另一程序中打开// 其他文件夹中打开
    - 解决办法: 任务管理器-性能-资源监视器-CPU-关联的句柄搜索框-[输入文件名/文件夹名]-结束列出的所有任务
- PC端微信的"设置","备份"功能
    - 设置: 
        1. 设置-通用设置-[我是只保留了: 1. 保留聊天记录; 2. 适配比例; 3. 使用默认浏览器打开网页]
        2. 设置-[在备份完成后]-清空聊天记录
    - 备份: [每个星期]备份至电脑
    - Android微信客户端: [进入"我-设置"]
        1. 聊天-聊天记录备份与迁移-清空聊天记录
        2. 通用-字体大小-最小
        3. 通用-照片视频与文件-全部关闭
        4. 通用-发现页管理-只保留"朋友圈"+"小程序"
        5. 通用-横屏模式+NFC功能-关闭
- Jupyter notebook 快捷方式
    - 目标是: 1. work_dir换成D:/jupyter notebook 2. 用conda命令行输入jn打开jupyter notebook[此时其work_dir是在D:/jupyter notebook]
    - 解决方法:
        1. conda输入jupyter notebook --generate-config, 找到jupyter_notebook_config.py, 查找c.NotebookApp.notebook_dir, 填写保存
        2. [改名] 利用https://stackoverflow.com/questions/20530996/aliases-in-windows-command-prompt下的Velixo的办法, 创建文件夹D:/aliases, 里面写一个jn.bat, 内容是: # jn就是你的aliase
            - @echo off
            - echo.
            - jupyter notebook %*
- 换行, 回车是两个不同的概念!
    - 换行: \n -> newline; 表示光标下移一行[不一定在行首]
    - 回车: \r -> return; 表示光标回到开头字符处; [就有的时候没有换行就直接回车 可能会覆盖掉之前的字符吧估计]
- java定义数组风格是: datatype[] arrayrefvar; C++/C定义数组风格是: datatype arrayrefvar[]; 

- pycharm的project interpretr 安装包时nothing to show: 第三个按钮刷新一下

- 单行速度查询: profiling
   

 
        
    
  
