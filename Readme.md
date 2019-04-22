链接：https://www.zhihu.com/question/42017514/answer/116565949

目前市面上安卓模拟器软件看着种类繁多，但其实只有两大流派：
Bluestacks和Virutalbox。Bluestacks的历史可以追溯到2011年，
是最早在PC上实现流畅运行安卓系统的方案。
Bluestacks的原理是把Android底层API接口翻译成Windows API，对PC硬件本身没有要求，
在硬件兼容性方面有一定的优势。但Bluestacks需要翻译的Android接口数量巨大，很难面面俱到，
而且存在软件翻译的开销，在性能和游戏兼容性方面欠佳。
Virtualbox是数据库巨头Oracle旗下的开源项目，
通过在Windows内核底层直接插入驱动模块，创建一个完整虚拟的电脑环境运行安卓系统，加上CPU VT硬件加速，性能和兼容性都更好，但是对于电脑CPU有一定要求，超过五年以上的电脑使用起来比较吃力。国内像靠谱助手、新浪手游助手等一大批手游助手类都是直接基于Bluestacks内核，因为Bluestacks没有公开源代码无法深度定制，只能简单的优化，再包装界面后上市。其他的像海马玩、逍遥安卓、夜神、ITools这类的产品都是基于Virtualbox，能力弱的（如海马玩、ITools）直接采用Oracle发布的Virtualbox商业版，能力强的（如逍遥安卓、夜神）则对Virtualbox源代码深度定制后重新编译来进一步提高性能和兼容性。

vbox内核定制
夜神模拟器、雷电模拟器、逍遥、海马玩、靠谱助手、Genymotion