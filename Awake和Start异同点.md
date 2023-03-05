### Same:
+  两者都是对象初始化时调用的，都在Update之前，场景中的对象都生成后才会调用Awake，Awake调用完才会调用Start，所有Start调用完才会开始Update
<br>
+ 两者在对象生命周期内都只会被调用一次，即初始化时被调用，之后即使是在被重新激活之后也不会再次被调用

### Difference:
+ Awake函数在对象初始化之后立刻就会调用，换句话说，对象初始化之后第一调用的函数就是Awake；而Start是在对象初始化后，第一次Update之前调用的
<br>
+ 在 Start中进行初始化不是很安全，因为它可能被其他自定义的函数抢先
<br>
+ 在 Start中进行初始化不是很安全，因为它可能被其他自定义的函数抢先
<br>
+ **Awake不管脚本是否enabled都会被调用；而Start如果对象被SetAcive(false)或者enabled= false了是不会被调用的;OnEnable会在Start之前执行** 
<br>
+ 如果对象（GameObject）本身没激活，那么Awake，Start都不会调用