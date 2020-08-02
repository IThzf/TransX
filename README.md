# TransX
使用tensorlfow实现TransX表示学习模型



├─data  // 数据集  
│  ├─embeddings
│  ├─FB15k     
│  └─YAGO39K
│      ├─M-Test   
│      ├─M-Valid    
│      ├─Test   
│      ├─Train  
│      └─Valid
│              
├─python  纯python实现的TransE及TransH
│  ├─TransE  已实现
│  │      Test_TransE.py
│  │      Train_TransE.py
│  │      
│  └─TransH   未完全实现
│          Test_TransH.py
│          Train_TransH.py
│          
├─Tensorflow  使用tensorflow实现的TransX模型
│  ├─data  存储训练好的模型
│  ├─embeddings  好像是多余的？
│  ├─TransC   TransC模型的实现及测试
│  │  │  Test_TransC_Classification_InstanceOf.py   InstanceOf类型的元组分类  
│  │  │  Test_TransC_Classification_Normal.py   Triple类型的三元组分类  
│  │  │  Test_TransC_Classification_SubClassOf.py subClassOf类型的元组分类  
│  │  │  Test_TransC_Link_Predication.py  Triple类型的三元组的链接预测  
│  │  │  Train_TransC.py   TransC模型实现第一版  
│  │  │  Train_TransC2.py  TransC模型实现第二版  
│  │  │  
│  │  └─embeddings  存储训练好的模型参数
│  │
│  ├─TransD  TransD模型
│  │      Test_TransD.py   测试
│  │      Train_TransD.py   训练
│  │      
│  ├─TransE  TransE模型
│  │  │  Test_TransE.py  测试
│  │  │  Train_TransE.py  训练
│  │  │  
│  │  └─checkpoint_dir  检查点文件
│  │
│  ├─TransH  TransH模型，含具体的代码注释
│  │  │  Test_TransH.py   TransH测试
│  │  │  Train_TransH.py  TransH训练
│  │  │  
│  │  └─checkpoint_dir  检查点文件
│  │
│  └─TransR  TransR模型
│          Test_TransR.py  TransR测试
│          Train_TransR.py TransR训练
│          
└─util   工具包
    │  file_util.py  文件读取工具，由于需要读取不同数据集和模型参数，目前方法较多，代码可读性貌似不高
    │  transform_nn.py  bern负样本生成方法，用于计算概率
    │  __init__.py  初始化文件
    │  
    └─__pycache__
