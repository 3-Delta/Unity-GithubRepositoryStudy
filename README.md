# Unity-GithubRepositoryStudy

1. https://github.com/jynew/jynew    
2. https://unitylist.com/p/fpi/Unity-toolbar-extender                              
        1. Editor下模型预览的实现
        2. Editor下快速查看Id对应的Icon的机制
        3. 编辑器自定义P的播放按钮
        4. UI节点分层
2. https://github.com/egametang/ET                           
        1. 同步上下文的机制
        2. Task以及MethodBuilder的机制
        3. UpdateComponent作为组件驱动Entity的Update的装饰者模式，可以用该模式使用NetReconnect组件
3. https://github.com/kaclok/Game-Programmer-Study-Notes  学习笔记
4. https://github.com/kaclok/SceneSeparateDemo                                
        1. 4叉树场景分隔管理            
5. https://github.com/yiv/blog                                     
        1. 网络同步                 
6. https://github.com/kaclok/Books                                      
        1. Gpu以及shader介绍        
7. https://github.com/MEyes/uMVVM                                        
        1. MVVM的机制          
8. https://github.com/sundxing/Unity-Excpetion-Crash                         
        1. Unity/Android/iOS的异常处理机制， 以及对于异常堆栈的解析流程，比如安卓的addr2line的工具

9. urp的卡通渲染 https://unitylist.com/p/106r/URP-Toon 多对象的多pass的渲染顺序与内置管线的区别
10. https://github.com/xasset/xasset  https://xasset.github.io/#/preload  
        1. 异步转同步实现
        2. 下载限速
        3. editor下使用分桢的同步加载模拟异步加载
        4. 本地不存在资源会远程加载
11. https://github.com/Cysharp/ZString 
        1. zerostring的实现，以及.github/workflows/build-debug.yml中关于特定Unity版本的编译，打包成.unitypackage的操作，以及.net的编译环境
        2. 自动打包github的release package
        3. zerostring其实就是底层借助ArrayPool<char>.Shared.Rent存储string, 借助ReadOnlySpan<char>处理Append的传参， 但是tostring依然是每次new string一个新的string, 所以只是减少中间操作的垃圾，最终tostring的还是避免不了。 同时处理remove以及replace之类的时候，借助span快速处理
        
12. https://github.com/neon-age/Smart-Inspector， peek插件  多个并列组件的inspector只draw一个的实现
        
13. https://github.com/yasirkula/UnityNativeGallery  sdk获取相机图片
        
14. https://github.com/EllanJiang/GameFramework gameframework的ui机制，soundagent机制
        https://github.com/yimengfan/BDFramework.Core sqlit配置表
        
15. https://github.com/Unity-Technologies/BoatAttack 
        PlatformFramerateLock 限制物理帧以及渲染帧
        MiniProfiler，Benchmark cpu，内存，帧率等实时统计
        AppSettings.cs 动态分辨率的实现, UniversalRenderPipeline.asset.renderScale 或者 ScalableBufferManager.ResizeBuffers(offsetVec.x, offsetVec.y)
        DayNightController  日夜系统
        水面制作，水的交互，水浪的制作
        LocalToWorldJob 使用jobs并行计算，加速逻辑


