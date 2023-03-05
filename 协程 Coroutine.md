## yield

+ **yield return null;** //下一帧以后执行后续代码
  + 等待Update()中代码运行完成后执行后面的代码

+ **yield return 0;** //任意数字，同上
  + 等待Update()中代码运行完成后执行后面的代码

+ **yield break;** //直接终止，类似于return

+ **yield return StartCoroutine(Timer(1));** //等待一个携程运行完成

+ **yield return new  WaitForSeconds(任意数字);**
  + 等待对应秒数后执行后面的代码
  + 受到 timeScale 影响

+ **yield return new WaitForSecondsRealtime(任意数字);**
  + 等待对应秒数后执行后面的代码
  + 不受 timeScale 影响

+ **yield return WaitForEndOfFrame();**
  + 等待这一帧所有代码执行完成后执行后面的代码

+ **yield return WaitForEndOfFixedUpdate();**
  + 等待 FixedUpdate()中代码运行完成后执行后面的代码

+ **yield return new WaitUntil(()=> oneSecond>1);**
  + 等待某判断条件为真时

+ **yield return new WaitWhile(()=> oneSecond>1);**
  + 等待某判断条件为j假时

  
## 注意事项
+  携程需要用 IEnumerator (迭代器)命名其中必须包含 yield return 关键字

   +  StartCoroutine(携程方法)

   +  StopCoroutime(携程方法)  停止指定携程

   +  StopAllCoroutines()  停止全部携程

## 携程概念
+ 不是多线程，是一种异步多任务处理

![coroutine](/Images/coroutine.jpg)