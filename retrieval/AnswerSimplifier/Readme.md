内容简化器的实现。针对数据库返回的维基百科长文档，以句子为单位，找到最有可能出现答案的前几个句子，并排序返回。

使用方法：直接运行 AnswerSimplifier.exe 即可。已封装在了 main.py 中。

输入：同目录下的 input 和 output 文件，分别表示问题和长段落内容。

输出：同目录下的 ans.txt ，按句子相关度排序，每个问题之间有空行。

使用环境：  
（1）在同级目录下建立/tmp文件夹  
（2）在同级目录下包含ltp库，具体结构为  
/ltp  
├── ltp_data  
│   ├── cws.model  
│   ├── ner.model  
│   ├── parser.model  
│   └── pos.model  
├── ltp_test.exe  
├── cws_cmdline.exe  
├── ner_cmdline.exe  
├── par_cmdline.exe  
├── pos_cmdline.exe  
└── srl_cmdline.exe  
