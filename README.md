# mip-cli-plugin-miniprogram

MIP Cli 的插件，可以将小程序的页面转换为[百度智能小程序](https://smartprogram.baidu.com/developer/index.html)

## 使用方法

插件支持两种使用方式，URL 和本地的文件均可

```
$ npm install mip2
$ mip2 miniprogram --name index --dir . https://www.mipengine.org/
$ mip2 miniprogram --name index --dir /home/mipengine/miniprogram index.html
```

通过上面的命令将会在对应的目录生成转换好的小程序页面。

- 如果目标目录是小程序目录，则会在目录的 components 目录中插入引用的 MIP 自定义组件，同时在 pages 目录放入对应的页面
- 如果目标目录不是小程序目录，则会提示输入目录名，转换工具会创建一个目录，并将对应的文件写入目录中
