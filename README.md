# cartool

> Export images from OS X / iOS .car CoreUI archives.  
> Very rough code, probably tons wrong with it, but still useful.

---

* https://github.com/steventroughtonsmith/cartool
    * 代码 fork 于此
* 缺点
    * 只能 dump 出资源文件, 而不是 Assets.xcassets 格式
* 环境
    * xcode
        * Version 14.0.1 (14A400)
        * ![](https://cdn.jsdelivr.net/gh/HaoweiCh/imgs/28F181C89D5A852458037F10A8D8EE8B8F724946.webp)
    * macOS
        * 13.0
        * ![](https://cdn.jsdelivr.net/gh/HaoweiCh/imgs/FEF5420748847CECB8744810EFAC5C2C36FE8652.webp)

## 步骤

1. 拉本项目 `git clone --depth=1`
2. Command+B 编译
3. *Show Build folder in Finder*
    * ![](https://cdn.jsdelivr.net/gh/HaoweiCh/imgs/2BC3B0B70BDDDF5AA390C953BCE118BD359D0715.webp)
4. cp ./Products/Debug/cartool destination-you-want
    * 拷贝 cartool 到任何位置你喜欢的如 /usr/local/bin 就可以全局访问了
5. cartool Payloader/demo.app/Assets.car ./assets
    * 导出 Assets.car 的所有资源到 assets 目录下（记得提前创建 assets 目录哦）