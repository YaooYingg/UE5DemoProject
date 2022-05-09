# NoitomMetahumanTest 工程使用说明

1. 请使用UE5 官方引擎版本打开该工程
   
    ![01 UE5 version](https://user-images.githubusercontent.com/86640695/167243587-7e4076f8-8230-438d-b5a3-b38e89ed7ef2.jpg)

2. 工程打开后先应用以下插件：

   2.1 NeuronLiveLink v1.2.0.4 下载地址：https://github.com/pnmocap/NoitomMocapLiveLinkPlugin/releases/tag/v1.2.04
   
    ![02 NeuronLiveLink](https://user-images.githubusercontent.com/86640695/167243797-57a1618b-7561-44e3-ae8e-4f964a0dfe2f.jpg)

   
   2.2 其他引擎内置插件：RigLogic Plugin v7.0.5，Groom，Apple ARKit 和 Apple ARKit Face Support
   
    ![04 RigLogicPlugin](https://user-images.githubusercontent.com/86640695/167243801-48cfda80-78ae-462d-b544-8749097ec24a.jpg)
    ![05 GroomPlugin](https://user-images.githubusercontent.com/86640695/167243803-3fe67445-ad38-4e5c-8c99-9d1f31efbce1.jpg)
    ![03 Apple plugin](https://user-images.githubusercontent.com/86640695/167243804-40170c4a-95f7-4d92-a2cb-055e5f726b62.jpg)

   
3. 应用插件后需要重启工程，打开Live Link 窗口
   
    ![06 LiveLink window](https://user-images.githubusercontent.com/86640695/167243902-9186f673-09fb-4058-bc3f-fd5bef9d3d62.jpg)

4. 打开Axis Studio软件，连接动捕设备或者回放动捕数据，打开BVH 数据流开关
   
   4.1 使用录制文件时的数据流设置示例
   
     ![07 Axis Studio 设置](https://user-images.githubusercontent.com/86640695/167244115-2620de74-433d-458e-9342-214c59677224.jpg)
   
   4.2 连接动捕设备时的数据流设置示例
   
     ![08 Axis Studio 设置](https://user-images.githubusercontent.com/86640695/167244167-22809f6e-64b1-4cfd-9ecd-174cf95a3a5b.jpg)


5. 在Live Link 窗口中添加动捕数据源
     ![LiveLinkAddAxisStudioSource](https://user-images.githubusercontent.com/86640695/167246831-57a5c236-0be7-4781-89e1-bfd206a0b27b.gif)

6. 运行Live Link Face 软件，完成数据流连接设置，面捕数据流一旦连接成功后会自动在Live Link 窗口中完成数据源添加，不需要手动添加
     ![09 LiveLinkAddFaceSource](https://user-images.githubusercontent.com/86640695/167245247-8519392f-ad49-4208-bcfa-28eaa0235e4f.jpg)

7. Content 中打开示例场景 NoitomMetahumanTest
     ![OpenMap](https://user-images.githubusercontent.com/86640695/167246824-b115cd0c-423d-46d4-a046-8d5e390f5376.gif)

8. Content 中搜索 m_tal_nrw_animbp 动画蓝图并双击打开
     ![OpenBP](https://user-images.githubusercontent.com/86640695/167246836-e656d06b-ba88-4ca2-a63a-7044194ed467.gif)

9. AnimGraph 中为Live Link Pose 节点设置角色名称，然后点击Compile
     ![SetupChrName](https://user-images.githubusercontent.com/86640695/167246841-2e2a215c-d09e-44cd-8705-a5812b70459e.gif)

10. 场景中选中模型，在Datails >Default 面板中设置LLink Face subject
     ![SetupARFaceName](https://user-images.githubusercontent.com/86640695/167246842-12a0cbc7-89fc-4e58-aa05-752ce5d4ef4c.gif)

11.点击Play 运行即可查看全身+面捕驱动效果 
     ![Play](https://user-images.githubusercontent.com/86640695/167331440-91d2fe9a-0230-4832-b99b-37e667075e36.gif)
