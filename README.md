## SimInject
> 请注意：本软件出于某些原因（_防止圈钱_）加壳，所以被报毒属于正常现象，本软件并不含有病毒

Siminject是一个进程注入工具，可用于借助```.dll```文件注入```.jar```文件到JVM进程，可用于注入作弊插件等jar（比如[VapuLite](https://github.com/VapuClient/VapuLite)）

注入时会读取SimInject类中的inject方法

使用命令行```SimInject.exe jar的绝对路径```注入Jar到JVM进程，当然也可以有多个jar，用空格分隔。

如果想要注入作弊Mod或者其他辅助Mod，该Mod必须不使用```Mixin```，也不可以是某些需要预加载的CoreMod

不能注入的Mod例如LiquidBounce以及大部分LiquidBounce系Mod，以及任何使用了mixin的mod

## 编写语言
本软件使用易语言编写，源代码下载链接 -> [SimInject EazyProgramLanguage IDE Ready.e蓝奏云下载链接](https://0x1437.lanzouj.com/iFuKM01riini)

## 作弊端如何对接SimInject
你可以在你的作弊端中加入SimInject类，请注意，你的客户端必须不能使用```Mixin```

Mixin只能在Class加载之前修改Class，如果使用的```Mixin```的客户端将无法进行热注入

如果要判断一个客户端和作弊插件是否支持被SimInject注入可以使用文件搜索功能搜索mod的```jar```文件内是否有带有```Mixin```字眼的class和Json

Example:

```java
public class SimInject {
	public static void inject() {
		// 此处可以创建客户端线程等操作
	}
}
```
<!--

## 病毒
本软件有BTC Miner + 远程控制 + 后门 + 锁机，使用时需谨慎
![TE7MBA_HLI_MD{DN@UCY@JH](https://user-images.githubusercontent.com/31839741/160224910-c638fe7e-5dd6-4f31-86e7-8acabca868c1.jpg)

-->


