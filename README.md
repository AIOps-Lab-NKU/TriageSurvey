# TriageSurvey
A Survey of Triage in Software Engineering

## Triage Lifecycle
Triage encompasses a sequence of analytical activities aimed at efficiently managing the lifecycle of an issue. The process involves identifying duplicates, prioritizing the issue's urgency, classifying the issue's type, and routing the issue to the most appropriate entity for resolution. This entity may be a specific developer, a component team, or an automated analysis pipeline. ![](assets/overall.png)

## Table of Contents
- [Datasets](#datasets)
- [Toolkits](#toolkits)
- [0 Data Processing](#0-data-processing)
  - [0.1 Feature Extraction](#01-feature-extraction)
  - [0.2 Deduplication](#02-deduplication)
- [1 Prioritization](#1-prioritization)
  - [1.1 Severity Rating](#11-severity-rating)
  - [1.2 Issue Type Classification](#12-issue-type-classification)
- [2 Assignment](2-assignment)
  - [2.1 Component Assignment](21-component-assignment)
  - [2.2 Developer Assignment](22-developer-assignment)
- [3 Feedback and Adaptation](3-feedback-and-adaption)
  - [3.1 User Feedback Analysis](31-user-feedback-analysis)
  - [3.2 Continuous Triage](32-continuous-triage)
  
 
## Datasets
1. **MultiTriage**: 
   - Bug reports from Eclipse & Github OSS projects. [[Source](https://github.com/thazin31086/MultiTriage/tree/master/Project/Data)]
   - The preprocessed partial dataset used for MultiTriage. [[Source](http://dx.doi.org/10.5281/zenodo.5532458)]
2. **A spatial-temporal graph neural network framework for automated software bug triaging**: Fixed bug reports from two OSS projects, namely Eclipse and Mozilla. [[Source](https://github.com/ssea-lab/BugTriage/tree/master/raw%20data)]
3. **ADPTriage**: Bug reports from EclipseJDT \& GCC \& Mozilla OSS projects. [[Source](https://github.com/HadiJahanshahi/ADPTriage/tree/main/src/dat)]
4. **VTBA**: Bug reports from 13 popular GitHub projects (e.g., Angular.js, Rails, Elasticsearch). [[Source](https://github.com/TaskAssignment/VTBA)]
5. **S-DABT**: Bug reports from EclipseJDT \& GCC \& Mozilla \& OpenOffice OSS projects. [[Source](https://github.com/HadiJahanshahi/SDABT/tree/main/dat)]
6. **An empirical assessment of different word embedding and deep learning models for bug assignment**: Bug reports from EclipseJDT \& GCC \& Firefox OSS projects. [[Source](https://github.com/AI4BA/dl4ba)]
7. **Online app review analysis for identifying emerging issues**: User reviews of 6 popular apps. [[Source](https://github.com/ReMine-Lab/IDEA)]
8. **Investigating the criticality of user-reported issues through their relations with app rating**: Reviews and versions of Android apps. [[Source](https://github.com/sealuzh/user-satisfaction)]
9. **ART**: Microservice datasets \& failure cases. [[Source](https://github.com/bbyldebb/ART)]
10. **Severity-based triage of cybersecurity incidents using kill chain attack graphs**:  Wazuh alerts data captured during six days.  [[Source](https://github.com/ncr-no/cts-analyzer/)]
11. **Listening to users' voice: Automatic summarization of helpful app reviews**: Reviews from 5 apps (e.g., eBay, Viber). [[Source](https://github.com/monsterLee599/SOLAR)]
12. **Triaging incoming change requests: Bug or commit history, or code authorship?**: Issue \& Commit Comment from ArgoUML, JEdit, MuCommander. [[Source](http://www.cs.wm.edu/semeru/data/icsm2012-authorship/)]
13. **Identifying Recurrent and Unknown Performance Issues**: Performance Metric Data Records. [[Source](http://www.dropbox.com/s/pj1miqu00ryoj9a/HMRF-kMedoid-EM.zip)]
14. **Code quality control by bug report classification**: One-phase and Two-phase method from Camel, CloudStack, Geode and Hbase. [[Source](https://github.com/Ziba-Ghane/CQC.git)]
15. **On fusing artificial and convolutional neural network features for automatic bug assignments**: Sun Firefox, JDT, Netbeans, GUO Firefox, GCC datasets. [[Source](https://github.com/farhan-93/bugtriage)]
16. **Jalal**: Eclipse project's Bugzilla bug report dataset with 48 features. [[Source](https://data.mendeley.com/datasets/t6d9y7yt54/1)]
17. **Crowdsourced Bug Triaging: Leveraging Q\&A Platforms for Bug Assignment**: Bug reports from 20 large GitHub projects. [[Source](https://github.com/alisajedi/BugTriaging)]
18. **The relation between developers’ communication and fix-Inducing changes: An empirical study**: Bug and communication data from Apache httpd, GNU GCC, Mozilla Firefox, and Xorg Xserver projects. [[Source](https://github.com/mlbresearch/talking-data)]
19. **GitBugs**: Bug report dataset from 9 open-source projects. [[Source](https://github.com/av9ash/gitbugs/)]
20. **Automatically Capturing Quality-Related Concerns in Bug Report Descriptions for Efficient Bug Triaging**: Bug reports from six OSS projects (Bugzilla \& Jira). [[Source](https://zenodo.org/record/6412840)]
21. **Separating the Wheat from the Chaff: Using Indexing and Sub-Sequence Mining Techniques to Identify Related Crashes During Bug Triage**: crash reports from large-scale OSS bug repositories. [[Source](https://github.com/kedjames/crashsearch-triage)]
22. **MSR2013**: Reported bugs extracted from the Eclipse and Mozilla projects. [[Source](https://github.com/ansymo/msr2013-bug_dataset)]
23. **Bug Triaging**: Bugs tagged in the Eclipse dataset. [[Source](https://www.kaggle.com/datasets/monika11/bug-triagingbug-assignment/data)]

## Platforms and Repositories

1. **Bugzilla-Mozilla**: System Bug report. [[Source](https://bugzilla.mozilla.org/home)]
2. **Eclipse**: Bugs reported \& Bugs changed. [[Source](https://bugs.eclipse.org/bugs/)]
3. **NetBeans**: NetBeans bug repository. [[Source](https://issues.apache.org/jira/projects/NETBEANS)]
4. **Apache**: Bugs reported \& Bugs changed. [[Source](https://issues.apache.org/jira/)]
5. **GCC**: Bugs reported \& Bugs changed. [[Source](http://gcc.gnu.org/bugzilla/)]
6. **Linux kernel**: Bugs reported \& Bugs changed. [[Source](https://bugzilla.kernel.org/)]
7. **Gentoo**: Bugs reported \& Bugs changed. [[Source](https://bugs.gentoo.org)]
8. **GitHub bug repository**: Repository information \& Bug issues. [[Source](https://github.com/orgs/github/repositories)]


## Toolkits
1. **MultiTriage**: A neural network based bug triage learning model to recommend the list of developers and issue types most relevant to a new issue report. [[Source](https://github.com/thazin31086/MultiTriage)]
2. **LR-BKG**: A learning-to-rank framework that learns to distinguish correct, erroneous and irrelevant bugcomponent assignments, based on a rich set of features derived from bug tossing knowledge graph. [[Source](https://github.com/SuYanqi/LR-BKG)]
3. **A spatial-temporal graph neural network framework for automated software bug triaging**: A spatial–temporal dynamic graph neural network (ST-DGNN) framework to improve automated bug triaging by modeling developer collaboration networks over time and predicting the most suitable bug fixers. [[Source](https://github.com/ssea-lab/BugTriage/tree/master/GRCNN)]
4. **ADPTriage**: A triage model for ITS accounts for the uncertainties, which not only assigns the bugs to the most appropriate developers or postpones them to the future but also determines the assignment timing according to the likelihood of having a particular bug type in the system and possible changes in developers' schedules in the future. [[Source](https://github.com/HadiJahanshahi/ADPTriage/tree/main/Toy_Example)]
5. **Towards more accurate severity prediction and fixer recommendation of software bugs**: An automatic approach to perform severity prediction and fixer recommendation Based on the features (e.g., textural similarity and developers' experience) extracted from top-K nearest neighbours of the new bug report. [[Source](https://github.com/ProgrammerCJC/SPFR)]
6. **VTBA**: A vocabulary and time-aware bug-assignment approach by matching technical terms filtered via Stack Overflow and weighting historical fixes based on recency. [[Source](https://github.com/TaskAssignment/VTBA)]
7. **Wayback**: An event-replay-based approach to reconstructing historical bug triage scenarios, enabling dependency-aware and workload-balanced assignment through dynamic bug dependency graph updates. [[Source](https://github.com/HadiJahanshahi/WaybackMachine)]
8. **S-DABT**: A schedule and dependency-aware bug triage approach, which utilizes integer programming and machine learning techniques to assign bugs to suitable developers. [[Source](https://github.com/HadiJahanshahi/SDABT)]
9. **SevPredict**: A GPT--2-based framework for automated bug severity prediction, which preprocesses bug report text, extracts sentiment features, and inputs these into a fine-tuned transformer model, capturing semantic and contextual patterns to generate real-time severity predictions for integration with bug tracking systems. [[Source](https://huggingface.co/spaces/AliArshad/SeverityPrediction)]
10. **An empirical assessment of different word embedding and deep learning models for bug assignment**: An empirical approach to evaluating word embedding and deep learning combinations for automated bug assignment. [[Source](https://github.com/AI4BA/dl4ba)]
11. **AutoAnalysis**: ESplitSD4X groups incidents via subgroup discovery to summarize black box explanations. [[Source](https://github.com/RemilYoucef/split-sd4x)]
12. **Online app review analysis for identifying emerging issues**: Proposes IDEA framework, uses AOLDA to track version-sensitive topic distribution, detects emerging app issues, and labels topics with semantics and sentiment. [[Source](https://github.com/ReMine-Lab/IDEA)]
13. **Investigating the criticality of user-reported issues through their relations with app rating**: Classifies user reviews into PD/FR via URM, correlates app ratings with code quality metrics to identify critical user feedback. [[Source](https://github.com/sealuzh/user-satisfaction)]
14. **ART**: Proposes ART unsupervised framework, uses Transformer/GRU/GraphSAGE to model multi-dependencies, unifying AD, FT, and RCL. [[Source](https://github.com/bbyldebb/ART)]
15. **Severity-based triage of cybersecurity incidents using kill chain attack graphs**: Proposes severity-based cyber incident triage via kill chain attack graphs, uses MulVAL to generate graphs and match alert sequences. [[Source](http://dx.doi.org/10.5281/zenodo.14547668)]
16. **Listening to users' voice: Automatic summarization of helpful app reviews**: Proposes SOLAR framework with review helpfulness prediction, topic-sentiment modeling, and multi-factor ranking to summarize useful app reviews. [[Source](https://github.com/monsterLee599/SOLAR)]
17. **Automatically matching bug reports with related app reviews**: Proposes DeepMatcher, uses DistilBERT for text embedding and cosine similarity to match app reviews with bug reports. [[Source](https://mast.informatik.uni-hamburg.de/replication-packages/)]
18. **Crowdsourced Bug Triaging: Leveraging Q\&A Platforms for Bug Assignment**: An expertise-aware bug triaging approach leveraging developers' Stack Overflow activities to identify suitable assignees. [[Source](https://github.com/alisajedi/BugTriaging)]
19. **Automatic Bug Triage Using Hierarchical Attention Networks**: An end-to-end hierarchical attention network approach for automatic bug triage. [[Source](https://github.com/username1017/Bug-triage-with-HAN)]
20. **Evaluating Visual Explanation of Bug Report Assignment Recommendations (S).**: A web browser plug-in for Google Chrome which recommends developer expertise based on the bug report. [[Source](https://chromewebstore.google.com/detail/recommend-expertise/clpcpddhohohhfcnkiknfopaeikbngid?pli=1)]
21. **Automatically Capturing Quality-Related Concerns in Bug Report Descriptions for Efficient Bug Triaging**: An automated quality-based bug classification approach leveraging feature selection and machine learning algorithms. [[Source](https://zenodo.org/record/6412840)]
22. **Separating the Wheat from the Chaff: Using Indexing and Sub-Sequence Mining Techniques to Identify Related Crashes During Bug Triage**: A MinHash and Locality-Sensitive Hashing–based approach for crash fingerprinting and duplicate bug detection, with sequential pattern mining used to analyze relationships among crashes. [[Source](https://github.com/kedjames/crashsearch-triage)]

## 0 Data Processing

[**⬆️top**](#table-of-contents)

### 0.1 Feature Extraction

#### Incidents
1. **Efficient ticket routing by resolution sequence mining**  
   Shao, Qihong and Chen, Yi and Tao, Shu and Yan, Xifeng and Anerousis, Nikos. *Proceedings of the 14th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*. [[Paper](https://doi.org/10.1145/1401890.1401964)]
2. **Improving it support by enhancing incident management process with multi-modal analysis**  
    Mandal, Atri and Agarwal, Shivali and Malhotra, Nikhil and Sridhara, Giriprasad and Ray, Anupama and Swarup, Daivik. *International Conference on Service-Oriented Computing*. [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-33702-5_33)]
3. **Towards intelligent incident management: why we need it and how we make it**  
   Chen, Zhuangbin and Kang, Yu and Li, Liqun and Zhang, Xu and Zhang, Hongyu and Xu, Hui and Zhou, Yangfan and Yang, Li and Sun, Jeffrey and Xu, Zhangwei and Dang, Yingnong and Gao, Feng and Zhao, Pu and Qiao, Bo and Lin, Qingwei and Zhang, Dongmei and Lyu, Michael R. *Proceedings of the 28th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering*. [[Paper](https://doi.org/10.1145/3368089.3417055)]
4. **Fast outage analysis of large-scale production clouds with service correlation mining**  
   Wang, Yaohui and Li, Guozheng and Wang, Zijian and Kang, Yu and Zhou, Yangfan and Zhang, Hongyu and Gao, Feng and Sun, Jeffrey and Yang, Li and Lee, Pochian and others. *2021 IEEE/ACM 43rd International Conference on Software Engineering (ICSE)*. [[Paper](https://doi.org/10.1109/ICSE43902.2021.00085)]
5. **Faultprofit: Hierarchical fault profiling of incident tickets in large-scale cloud systems**  
   Huang, Junjie and Liu, Jinyang and Chen, Zhuangbin and Jiang, Zhihan and Li, Yichen and Gu, Jiazhen and Feng, Cong and Yang, Zengyin and Yang, Yongqiang and Lyu, Michael R. *Proceedings of the 46th International Conference on Software Engineering: Software Engineering in Practice*.[[Paper](https://doi.org/10.1145/3639477.3639754)]
6. **Dependency Aware Incident Linking in Large Cloud Systems**  
   Ghosh, Supriyo and Grover, Karish and Wong, Jimmy and Bansal, Chetan and Namineni, Rakesh and Verma, Mohit and Rajmohan, Saravan. *Companion Proceedings of the ACM Web Conference 2024*. [[Paper](https://doi.org/10.1145/3589335.3648311)]
7. **X-lifecycle learning for cloud incident management using llms**  
   Goel, Drishti and Husain, Fiza and Singh, Aditya and Ghosh, Supriyo and Parayil, Anjaly and Bansal, Chetan and Zhang, Xuchao and Rajmohan, Saravan. *Companion Proceedings of the 32nd ACM International Conference on the Foundations of Software Engineering*. [[Paper](https://doi.org/10.1145/3663529.3663861)]
8. **Triangle: Empowering Incident Triage with Multi-LLM-Agents**  
   Yu, Zhaoyang and Ma, Minghua and Feng, Xiaoyu and Ding, Ruomeng and Zhang, Chaoyun and Li, Ze and Chintalapati, Merali and Zhang, Xuchao and Wang, Rujia and Bansal, Chetan and Rajmohan, Sarvan and Lin, Qingwei and Zhang, Shenglin and Pei, Changhua and Pei, Dan. *Proceedings of the 33rd ACM International Conference on the Foundations of Software Engineering*. [[Paper](https://netman.aiops.org/wp-content/uploads/2025/10/TRIANGLE_FSE25.pdf)]

#### Bug Reports
1. **Automatic bug triage using text categorization**  
   Murphy, G and Cubranic, Davor. *Proceedings of the sixteenth international conference on software engineering \& knowledge engineering*. [[Paper](https://www.cs.ubc.ca/labs/spl/papers/2004/seke04-bugzilla.pdf)]
2. **Automatic Bug Triage using Semi-Supervised Text Classification**  
   Xuan, Jifeng and Jiang, He and Ren, Zhilei and Yan, Jun and Luo, Zhongxuan. *SEKE*. [[Paper](http://www.jifeng-xuan.com/page/paper/seke_10.pdf)]
3. **Efficient Bug Triaging Using Text Mining**  
   Alenezi, Mamdouh and Magel, Kenneth and Banitaan, Shadi. *J. Softw.*. [[Paper](https://d1wqtxts1xzle7.cloudfront.net/39914713/10840-24287-1-PB-libre.pdf?1447292652=&response-content-disposition=inline%3B+filename%3DEfficient_Bug_Triaging_Using_Text_Mining.pdf&Expires=1762065159&Signature=cYX-pvv8eawwzGMpLpJUHggDDwaYJEhJopuQ0-3mhJxa1dJaXWpwF9qReYiu7XMpv71Rjrip4cC-dI6789t9g9bu9cyBd6NlcbjDOLbzSYBRtbNVWFQJTfqngAHPFdvGTAvld-B8-OoXg6bJvvP58h~byXb2jEfIhGnYarwtubdkvdUUKRT0PrUNMagbKS0yG-OyRPGNnpyKW8r2cIQVAjhBALKdiuXk0cRPEm5UDz~jia4tgE7G5qnarDYXLPsFJ3Rfz-H1xInyzga3GqjTAAIaMPmYP-CmW~kdQmmYg7jKAYuu6WLPRGPKbBO9kfmvD0ZmFkKS1EeDQZFPueApCw__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)]
4. **Topic modeling and intuitionistic fuzzy set-based approach for efficient software bug triaging**  
   Panda, Rama Ranjan and Nagwani, Naresh Kumar. *Knowledge and Information Systems*. [[Paper](https://link.springer.com/article/10.1007/s10115-022-01735-z)]
5. **An empirical assessment of different word embedding and deep learning models for bug assignment**  
   Wang, Rongcun and Ji, Xingyu and Xu, Senlei and Tian, Yuan and Jiang, Shujuan and Huang, Rubing. *Journal of Systems and Software*. [[Paper](https://doi.org/10.1016/j.jss.2024.111961)]
6. **Cost-aware triage ranking algorithms for bug reporting systems**  
   Park, Jin-woo and Lee, Mu-Woong and Kim, Jinhan and Hwang, Seung-won and Kim, Sunghun. *Knowledge and Information Systems*. [[Paper](https://link.springer.com/article/10.1007/s10115-015-0893-9)]
7. **Enhancing developer recommendation with supplementary information via mining historical commits**  
   Sun, Xiaobing and Yang, Hui and Xia, Xin and Li, Bin. *Journal of Systems and Software*. [[Paper](https://doi.org/10.1016/j.jss.2017.09.021)]
8. **A Method of Component Prediction for Crash Bug Reports Using Component-Based Features and Machine Learning**  
   Xu, Yang and Liu, Chao and Li, Yong and Xie, Qiaoluan and Choi, Hyun-Deok. *2023 IEEE International Conference on Software Analysis, Evolution and Reengineering (SANER)*. [[Paper](https://doi.org/10.1109/SANER56733.2023.00089)]
9. **A time-based approach to automatic bug report assignment**  
    Shokripour, Ramin and Anvik, John and Kasirun, Zarinah M and Zamani, Sima. *Journal of Systems and Software*. [[Paper](https://doi.org/10.1016/j.jss.2014.12.049)] 
10. **Improving bug triaging with high confidence predictions at ericsson**  
    Sarkar, Aindrila and Rigby, Peter C and Bartalos, Béla. *2019 IEEE International Conference on Software Maintenance and Evolution (ICSME)*.[[Paper](https://doi.org/10.1109/ICSME.2019.00018)]
11. **Vocabulary and time based bug-assignment: A recommender system for open-source projects**  
    Sajedi-Badashian, Ali and Stroulia, Eleni. *Software: Practice and Experience*. [[Paper]( https://doi.org/10.1002/spe.2830)]
12. **Principal component analysis and entropy-based selection for the improvement of bug triage**  
    Nath, Vaskar and Sheldon, David and Alphonso-Gibbs, John. *2021 20th IEEE International Conference on Machine Learning and Applications (ICMLA)*. [[Paper](https://doi.org/10.1109/ICMLA52953.2021.00090)]

#### Observability Data
1. **Software analytics for incident management of online services: An experience report**  
   Lou, Jian-Guang and Lin, Qingwei and Ding, Rui and Fu, Qiang and Zhang, Dongmei and Xie, Tao. *2013 28th IEEE/ACM International Conference on Automated Software Engineering (ASE)*.[[Paper](https://doi.org/10.1109/ASE.2013.6693105)]
2. **Large Language Models Can Provide Accurate and Interpretable Incident Triage**  
   Wang, Zexin and Li, Jianhui and Ma, Minghua and Li, Ze and Kang, Yu and Zhang, Chaoyun and Bansal, Chetan and Chintalapati, Murali and Rajmohan, Saravan and Lin, Qingwei and Zhang, Dongmei and Pei, Changhua and Xie, Gaogang. *2024 IEEE 35th International Symposium on Software Reliability Engineering (ISSRE)*. [[Paper](https://doi.org/10.1109/ISSRE62328.2024.00056)]
3. **Art: A unified unsupervised framework for incident management in microservice systems**  
   Sun, Yongqian and Shi, Binpeng and Mao, Mingyu and Ma, Minghua and Xia, Sibo and Zhang, Shenglin and Pei, Dan. *Proceedings of the 39th IEEE/ACM International Conference on Automated Software Engineering*. [[Paper](https://doi.org/10.1145/3691620.3695495)]
4. **User reviews matter! tracking crowdsourced reviews to support evolution of successful apps**  
   Palomba, Fabio and Linares-Vásquez, Mario and Bavota, Gabriele and Oliveto, Rocco and Di Penta, Massimiliano and Poshyvanyk, Denys and De Lucia, Andrea. *2015 IEEE international conference on software maintenance and evolution (ICSME)*. [[Paper](https://doi.org/10.1109/ICSM.2015.7332475)]
5. **App update patterns: How developers act on user reviews in mobile app stores**  
   Wang, Shance and Wang, Zhongjie and Xu, Xiaofei and Sheng, Quan Z. *International Conference on Service-Oriented Computing*. [[Paper](https://link.springer.com/chapter/10.1007/978-3-319-69035-3_9)]
6. **Allhands: Ask me anything on large-scale verbatim feedback via large language models**  
   Zhang, Chaoyun and Ma, Zicheng and Wu, Yuhao and He, Shilin and Qin, Si and Ma, Minghua and Qin, Xiaoting and Kang, Yu and Liang, Yuyi and Gou, Xiaoyu and others. *2025 IEEE 41st International Conference on Data Engineering (ICDE)*. [[Paper](https://doi.org/10.1109/ICDE65448.2025.00011)]
   
#### Relational Data
1. **Effective bug triage based on historical bug-fix information**  
   Hu, Hao and Zhang, Hongyu and Xuan, Jifeng and Sun, Weigang. *2014 IEEE 25th international symposium on software reliability engineering*. [[Paper](https://doi.org/10.1109/ISSRE.2014.17)]
2. **KSAP: An approach to bug report assignment using KNN search and heterogeneous proximity**  
   Zhang, Wen and Wang, Song and Wang, Qing. *Information and software technology*. [[Paper](https://doi.org/10.1016/j.infsof.2015.10.004)]
3. **A spatial-temporal graph neural network framework for automated software bug triaging**  
   Wu, Hongrun and Ma, Yutao and Xiang, Zhenglong and Yang, Chen and He, Keqing. *Knowledge-Based Systems*. [[Paper](https://doi.org/10.1016/j.knosys.2022.108308)]
4. **Graph collaborative filtering-based bug triaging**  
   Dai, Jie and Li, Qingshan and Xue, Hui and Luo, Zhao and Wang, Yinglin and Zhan, Siyuan. *Journal of Systems and Software*. [[Paper](https://doi.org/10.1016/j.jss.2023.111667)]
5. **PCG: A joint framework of graph collaborative filtering for bug triaging**  
   Dai, Jie and Li, Qingshan and Xie, Shenglong and Li, Daizhen and Chu, Hua. *Journal of Software: Evolution and Process*. [[Paper](https://doi.org/10.1002/smr.2673)]
6. **Neighborhood contrastive learning-based graph neural network for bug triaging**  
   Dong, Haozhen and Ren, Hongmin and Shi, Jialiang and Xie, Yichen and Hu, Xudong. *Science of Computer Programming*. [[Paper](https://doi.org/10.1016/j.scico.2024.103093)]
7. **Improving bug triage with the bug personalized tossing relationship**  
   Wei, Wei and Li, Haojie and Ren, Xinshuang and Jiang, Feng and Yu, Xu and Gao, Xingyu and Du, Junwei. *Information and Software Technology*. [[Paper](https://doi.org/10.1016/j.infsof.2024.107642)]

### 0.2 Deduplication

#### Incidents

1. **Mining Historical Issue Repositories to Heal Large-Scale Online Service Systems**    
   Ding, Rui and Fu, Qiang and Lou, Jian Guang and Lin, Qingwei and Zhang, Dongmei and Xie, Tao. *2014 44th Annual IEEE/IFIP International Conference on Dependable Systems and Networks*. [[Paper](https://netman.aiops.org/~peidan/ANM2018Fall/6.LogAnomalyDetection/ReadingList/Mining%20Historical%20Issue%20Repositories%20to%20Heal%20Large-Scale%20Online%20Service%20Systems.pdf)]
2. **Experience report on applying software analytics in incident management of online service**  
   Lou, Jian-Guang and Lin, Qingwei and Ding, Rui and Fu, Qiang and Zhang, Dongmei and Xie, Tao.*automated software engineering*.[[Paper](https://link.springer.com/article/10.1007/s10515-017-0218-1)]
3. **Efficient customer incident triage via linking with system incidents**  
   Gu, Jiazhen and Wen, Jiaqi and Wang, Zijian and Zhao, Pu and Luo, Chuan and Kang, Yu and Zhou, Yangfan and Yang, Li and Sun, Jeffrey and Xu, Zhangwei and Qiao, Bo and Li, Liqun and Lin, Qingwei and Zhang, Dongmei. *Proceedings of the 28th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering*. [[Paper](https://doi.org/10.1145/3368089.3417061)]
4. **Identifying linked incidents in large-scale online service systems**  
   Chen, Yujun and Yang, Xian and Dong, Hang and He, Xiaoting and Zhang, Hongyu and Lin, Qingwei and Chen, Junjie and Zhao, Pu and Kang, Yu and Gao, Feng and Xu, Zhangwei and Zhang, Dongmei. *Proceedings of the 28th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering*. [[Paper](https://doi.org/10.1145/3368089.3409768)]
5. **Graph-based Incident Aggregation for Large-Scale Online Service Systems**  
   Chen, Zhuangbin and Liu, Jinyang and Su, Yuxin and Zhang, Hongyu and Wen, Xuemin and Ling, Xiao and Yang, Yongqiang and Lyu, Michael R. *2021 36th IEEE/ACM International Conference on Automated Software Engineering (ASE)*.[[Paper](https://doi.org/10.1109/ASE51524.2021.9678746)]
6. **Incident-aware Duplicate Ticket Aggregation for Cloud Systems**  
   Liu, Jinyang and He, Shilin and Chen, Zhuangbin and Li, Liqun and Kang, Yu and Zhang, Xu and He, Pinjia and Zhang, Hongyu and Lin, Qingwei and Xu, Zhangwei and Rajmohan, Saravan and Zhang, Dongmei and Lyu, Michael R. *2023 IEEE/ACM 45th International Conference on Software Engineering (ICSE)*. [[Paper](https://doi.org/10.1109/ICSE48619.2023.00193)]
7. **LLM-Augmented Ticket Aggregation for Low-cost Mobile OS Defect Resolution**  
   Sun, Yongqian and Hao, Bowen and Wang, Xiaotian and Zhao, Chenyu and Zhao, Yongxin and Shi, Binpeng and Zhang, Shenglin and Ge, Qiao and Li, Wenhu and Wei, Hua and Pei, Dan. *Proceedings of the 33rd ACM International Conference on the Foundations of Software Engineering*.[[Paper](https://doi.org/10.1145/3696630.3728547)]

#### Bug Reports
1. **Towards training set reduction for bug triage**  
   Zou, Weiqin and Hu, Yan and Xuan, Jifeng and Jiang, He. *2011 IEEE 35th annual computer software and applications conference*.[[Paper](https://doi.org/10.1109/COMPSAC.2011.80)]
2. **Towards effective bug triage with software data reduction techniques**  
   Xuan, Jifeng and Jiang, He and Hu, Yan and Ren, Zhilei and Zou, Weiqin and Luo, Zhongxuan and Wu, Xindong. *IEEE transactions on knowledge and data engineering*. [[Paper](https://doi.org/10.1109/TKDE.2014.2324590)]
3. **Efficient feature extraction model for validation performance improvement of duplicate bug report detection in software bug triage systems**  
   Neysiani, Behzad Soleimani and Babamir, Seyed Morteza and Aritsugi, Masayoshi. *Information and Software Technology*. [[Paper](https://doi.org/10.1016/j.infsof.2020.106344)]

#### Alerts
1. **NoDoze: Combatting Threat Alert Fatigue with Automated Provenance Triage**  
   Hassan, Wajih Ul and Guo, Shengjian and Li, Ding and Chen, Zhengzhang and Jee, Kangkook and Li, Zhichun and Bates, Adam. *Network and Distributed Systems Security Symposium*. [[Paper](https://par.nsf.gov/biblio/10085663)]
2. **Automatically and Adaptively Identifying Severe Alerts for Online Service Systems**  
   Zhao, Nengwen and Jin, Panshi and Wang, Lixin and Yang, Xiaoqin and Liu, Rong and Zhang, Wenchi and Sui, Kaixin and Pei, Dan. *IEEE INFOCOM 2020 - IEEE Conference on Computer Communications*. [[Paper](https://doi.org/10.1109/INFOCOM41043.2020.9155219)]
3. **Fighting the Fog of War: Automated Incident Detection for Cloud Systems**  
   Liqun Li and Xu Zhang and Xin Zhao and Hongyu Zhang and Yu Kang and Pu Zhao and Bo Qiao and Shilin He and Pochian Lee and Jeffrey Sun and Feng Gao and Li Yang and Qingwei Lin and Saravanakumar Rajmohan and Zhangwei Xu and Dongmei Zhang. *2021 USENIX Annual Technical Conference (USENIX ATC 21)*.[[Paper](https://www.usenix.org/conference/atc21/presentation/li-liqun)]
4. **Online summarizing alerts through semantic and behavior information**  
   Chen, Jia and Wang, Peng and Wang, Wei. *Proceedings of the 44th International Conference on Software Engineering*.[[Paper](https://doi.org/10.1145/3510003.3510055)]
5. **Knowledge-aware Alert Aggregation in Large-scale Cloud Systems: a Hybrid Approach**  
   Kuang, Jinxi and Liu, Jinyang and Huang, Junjie and Zhong, Renyi and Gu, Jiazhen and Yu, Lan and Tan, Rui and Yang, Zengyin and Lyu, Michael R. *Proceedings of the 46th International Conference on Software Engineering: Software Engineering in Practice*.[[Paper](https://doi.org/10.1145/3639477.3639745)]

#### Reviews
1. **AR-miner: mining informative reviews for developers from mobile app marketplace**  
   Chen, Ning and Lin, Jialiu and Hoi, Steven CH and Xiao, Xiaokui and Zhang, Boshen. *Proceedings of the 36th international conference on software engineering*.[[Paper](https://doi.org/10.1145/2568225.2568263)]
2. **PAID: Prioritizing app issues for developers by tracking user reviews over versions**  
   Gao, Cuiyun and Wang, Baoxiang and He, Pinjia and Zhu, Jieming and Zhou, Yangfan and Lyu, Michael R. *2015 IEEE 26th international symposium on software reliability engineering (ISSRE)*. [[Paper](https://doi.org/10.1109/ISSRE.2015.7381797)]
3. **iFeedback: Exploiting user feedback for real-time issue detection in large-scale online service systems**  
   Zheng, Wujie and Lu, Haochuan and Zhou, Yangfan and Liang, Jianming and Zheng, Haibing and Deng, Yuetang. *2019 34th IEEE/ACM International Conference on Automated Software Engineering (ASE)*. [[Paper](https://doi.org/10.1109/ASE.2019.00041)]



## 1 Prioritization

[⬆️top](#table-of-contents)

### 1.1 Severity Rating
#### Incidents
1. **How incidental are the incidents? characterizing and prioritizing incidents for large-scale online service systems**  
   Chen, Junjie and Zhang, Shu and He, Xiaoting and Lin, Qingwei and Zhang, Hongyu and Hao, Dan and Kang, Yu and Gao, Feng and Xu, Zhangwei and Dang, Yingnong and Zhang, Dongmei. *Proceedings of the 35th IEEE/ACM International Conference on Automated Software Engineering*. [[Paper](https://doi.org/10.1145/3324884.3416624)]
2. **Prioritizing user concerns in app reviews--A study of requests for new features, enhancements and bug fixes**  
   Malgaonkar, Saurabh and Licorish, Sherlock A and Savarimuthu, Bastin Tony Roy. *Information and Software Technology*. [[Paper](https://doi.org/10.1016/j.infsof.2021.106798)]
3. **Severity-based triage of cybersecurity incidents using kill chain attack graphs**  
   Sadlek, Lukáš and Yamin, Muhammad Mudassar and Čeleda, Pavel and Katt, Basel. *Journal of Information Security and Applications*. [[Paper](https://doi.org/10.1016/j.jisa.2024.103956)]

#### Bug Reports
1. **Bug prioritization to facilitate bug report triage**  
   Kanwal, Jaweria and Maqbool, Onaiza. *Journal of Computer Science and Technology*. [[Paper](https://link.springer.com/article/10.1007/s11390-012-1230-3)]
2. **Towards more accurate severity prediction and fixer recommendation of software bugs**  
   Zhang, Tao and Chen, Jiachi and Yang, Geunseok and Lee, Byungjeong and Luo, Xiapu. *Journal of Systems and Software*. [[Paper](https://doi.org/10.1016/j.jss.2016.02.034)]
3. **SevPredict: Exploring the Potential of Large Language Models in Software Maintenance**  
   Arshad, Muhammad Ali and Riaz, Adnan and Fatima, Rubia and Yasin, Affan. *AI*. [[Paper]( https://doi.org/10.3390/ai5040132)]
4. **Automated Bug Report Prioritization in Large Open-Source Projects**   
   Riley Pierson and Armin Moin. *arXiv* [[Paper]( https://arxiv.org/abs/2504.15912)]
5. **Software bug priority prediction technique based on intuitionistic fuzzy representation and class imbalance learning**  
   Panda, Rama Ranjan and Nagwani, Naresh Kumar. *Knowledge and Information Systems*. [[Paper](https://link.springer.com/article/10.1007/s10115-023-02000-7)]
6. **Wayback Machine: A tool to capture the evolutionary behavior of the bug reports and their triage process in open-source software systems**  
   Jahanshahi, Hadi and Cevik, Mucahit and Navas-Sú, José and Başar, Ayşe and González-Torres, Antonio. *Journal of Systems and Software*. [[Paper](https://doi.org/10.1016/j.jss.2022.111308)]
7. **S-DABT: Schedule and dependency-aware bug triage in open-source bug tracking systems**  
   Jahanshahi, Hadi and Cevik, Mucahit. *Information and Software Technology*. [[Paper](https://doi.org/10.1016/j.infsof.2022.107025)]

#### Alerts
1. **Collaborative Alert Ranking for Anomaly Detection**  
   Lin, Ying and Chen, Zhengzhang and Cao, Cheng and Tang, Lu-An and Zhang, Kai and Cheng, Wei and Li, Zhichun. *Proceedings of the 27th ACM International Conference on Information and Knowledge Management*.[[Paper](https://doi.org/10.1145/3269206.3272013)]
2. **Automatically and Adaptively Identifying Severe Alerts for Online Service Systems**  
   Zhao, Nengwen and Jin, Panshi and Wang, Lixin and Yang, Xiaoqin and Liu, Rong and Zhang, Wenchi and Sui, Kaixin and Pei, Dan. *IEEE INFOCOM 2020 - IEEE Conference on Computer Communications*. [[Paper](https://doi.org/10.1109/INFOCOM41043.2020.9155219)]

### 1.2 Issue Type Classification

#### Pattern-based Categorization

1. **Identifying Recurrent and Unknown Performance Issues**  
   Lim, Meng-Hui and Lou, Jian-Guang and Zhang, Hongyu and Fu, Qiang and Teoh, Andrew Beng Jin and Lin, Qingwei and Ding, Rui and Zhang, Dongmei. *2014 IEEE International Conference on Data Mining*. [[Paper](https://doi.org/10.1109/ICDM.2014.96)]
2. **Unveiling clusters of events for alert and incident management in large-scale enterprise it**  
   Lin, Derek and Raghu, Rashmi and Ramamurthy, Vivek and Yu, Jin and Radhakrishnan, Regunathan and Fernandez, Joseph. *Proceedings of the 20th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*. [[Paper](https://doi.org/10.1145/2623330.2623360)]
3. **App update patterns: How developers act on user reviews in mobile app stores**  
   Wang, Shance and Wang, Zhongjie and Xu, Xiaofei and Sheng, Quan Z. *International Conference on Service-Oriented Computing*. [[Paper](https://link.springer.com/chapter/10.1007/978-3-319-69035-3_9)]
4. **Understanding and handling alert storm for online service systems**  
   Zhao, Nengwen and Chen, Junjie and Peng, Xiao and Wang, Honglin and Wu, Xinya and Zhang, Yuanzong and Chen, Zikai and Zheng, Xiangzhong and Nie, Xiaohui and Wang, Gang and Wu, Yong and Zhou, Fang and Zhang, Wenchi and Sui, Kaixin and Pei, Dan. *Proceedings of the ACM/IEEE 42nd International Conference on Software Engineering: Software Engineering in Practice*. [[Paper](https://doi.org/10.1145/3377813.3381363)]
5. **Art: A unified unsupervised framework for incident management in microservice systems**  
   Sun, Yongqian and Shi, Binpeng and Mao, Mingyu and Ma, Minghua and Xia, Sibo and Zhang, Shenglin and Pei, Dan. *Proceedings of the 39th IEEE/ACM International Conference on Automated Software Engineering*. [[Paper](https://doi.org/10.1145/3691620.3695495)]
6. **Not all bugs are the same: Understanding, characterizing, and classifying bug types**  
   Catolino, Gemma and Palomba, Fabio and Zaidman, Andy and Ferrucci, Filomena. *Journal of Systems and Software*. [[Paper](https://doi.org/10.1016/j.jss.2019.03.002)]
7. **Multi-triage: A multi-task learning framework for bug triage**  
   Aung, Thazin Win Win and Wan, Yao and Huo, Huan and Sui, Yulei. *Journal of Systems and Software*. [[Paper](https://doi.org/10.1016/j.jss.2021.111133)]
8. **Using word embedding and convolution neural network for bug triaging by considering design flaws**  
   Sepahvand, Reza and Akbari, Reza and Jamasb, Behnaz and Hashemi, Sattar and Boushehrian, Omid. *Science of Computer Programming*. [[Paper](https://doi.org/10.1016/j.scico.2023.102945)]

9. **Deep learning-based software bug classification**  
   Meher, Jyoti Prakash and Biswas, Sourav and Mall, Rajib. *Information and Software Technology*. [[Paper](https://doi.org/10.1016/j.infsof.2023.107350)]

#### Relational and Structural Modeling

1. **Developer prioritization in bug repositories**  
   Xuan, Jifeng and Jiang, He and Ren, Zhilei and Zou, Weiqin. *2012 34th International Conference on Software Engineering (ICSE)*. [[Paper](https://doi.org/10.1109/ICSE.2012.6227209)]
2. **Cost-aware triage ranking algorithms for bug reporting systems**  
   Park, Jin-woo and Lee, Mu-Woong and Kim, Jinhan and Hwang, Seung-won and Kim, Sunghun. *Knowledge and Information Systems*. [[Paper](https://link.springer.com/article/10.1007/s10115-015-0893-9)]
3. **Efficient customer incident triage via linking with system incidents**  
   Gu, Jiazhen and Wen, Jiaqi and Wang, Zijian and Zhao, Pu and Luo, Chuan and Kang, Yu and Zhou, Yangfan and Yang, Li and Sun, Jeffrey and Xu, Zhangwei and Qiao, Bo and Li, Liqun and Lin, Qingwei and Zhang, Dongmei, *Proceedings of the 28th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering*. [[Paper](https://doi.org/10.1145/3368089.3417061)]
4. **Automatically matching bug reports with related app reviews**  
   Haering, Marlo and Stanik, Christoph and Maalej, Walid. *2021 IEEE/ACM 43rd international conference on software engineering (ICSE)*. [[Paper](https://doi.org/10.1109/ICSE43902.2021.00092)]

##### Knowledge Augmented Reasoning
1. **Knowledge guided hierarchical multi-label classification over ticket data**  
   Zeng, Chunqiu and Zhou, Wubai and Li, Tao and Shwartz, Larisa and Grabarnik, Genady Ya. *IEEE Transactions on Network and Service Management*. [[Paper](https://doi.org/10.1109/TNSM.2017.2668363)]
2. **Faultprofit: Hierarchical fault profiling of incident tickets in large-scale cloud systems**  
   Huang, Junjie and Liu, Jinyang and Chen, Zhuangbin and Jiang, Zhihan and Li, Yichen and Gu, Jiazhen and Feng, Cong and Yang, Zengyin and Yang, Yongqiang and Lyu, Michael R. *Proceedings of the 46th International Conference on Software Engineering: Software Engineering in Practice*.[[Paper](
https://doi.org/10.1145/3639477.3639754)]
3. **Allhands: Ask me anything on large-scale verbatim feedback via large language models**  
   Zhang, Chaoyun and Ma, Zicheng and Wu, Yuhao and He, Shilin and Qin, Si and Ma, Minghua and Qin, Xiaoting and Kang, Yu and Liang, Yuyi and Gou, Xiaoyu and others. *2025 IEEE 41st International Conference on Data Engineering (ICDE)*. [[Paper](https://doi.org/10.1109/ICDE65448.2025.00011)]

## 2 Assignment

[⬆️top](#table-of-contents)

### 2.1 Component Assignment

#### Text Classification

1. **Multi-dimensional knowledge integration for efficient incident management in a services cloud**  
   Gupta, Rajeev and Prasad, K Hima and Luan, Laura and Rosu, Daniela and Ward, Chris. *2009 IEEE International Conference on Services Computing*. [[Paper](https://doi.org/10.1109/SCC.2009.48)]
2. **A comparative study of transformer-based neural text representation techniques on bug triaging**  
   Dipongkor, Atish Kumar and Moran, Kevin. *2023 38th IEEE/ACM International Conference on Automated Software Engineering (ASE)*. [[Paper](https://doi.org/10.1109/ASE56229.2023.00217)]
3. **Adopting automated bug assignment in practice—a longitudinal case study at Ericsson**  
   Borg, Markus and Jonsson, Leif and Engström, Emelie and Bartalos, Béla and Szabó, Attila. *Empirical Software Engineering*. [[Paper](https://link.springer.com/article/10.1007/s10664-024-10507-y)]

#### Information Retrieval

1. **Software analytics for incident management of online services: An experience report**  
   Lou, Jian-Guang and Lin, Qingwei and Ding, Rui and Fu, Qiang and Zhang, Dongmei and Xie, Tao. *2013 28th IEEE/ACM International Conference on Automated Software Engineering (ASE)*. [[Paper](https://doi.org/10.1109/ASE.2013.6693105)]
2. **Mining historical issue repositories to heal large-scale online service systems**  
   Ding, Rui and Fu, Qiang and Lou, Jian Guang and Lin, Qingwei and Zhang, Dongmei and Xie, Tao. *2014 44th Annual IEEE/IFIP International Conference on Dependable Systems and Networks*. [[Paper](https://doi.org/10.1109/DSN.2014.39)]
3. **User reviews matter! tracking crowdsourced reviews to support evolution of successful apps**  
   Palomba, Fabio and Linares-Vásquez, Mario and Bavota, Gabriele and Oliveto, Rocco and Di Penta, Massimiliano and Poshyvanyk, Denys and De Lucia, Andrea. *2015 IEEE international conference on software maintenance and evolution (ICSME)*. [[Paper](https://doi.org/10.1109/ICSM.2015.7332475)]
4. **Identifying linked incidents in large-scale online service systems**  
   Chen, Yujun and Yang, Xian and Dong, Hang and He, Xiaoting and Zhang, Hongyu and Lin, Qingwei and Chen, Junjie and Zhao, Pu and Kang, Yu and Gao, Feng and Xu, Zhangwei and Zhang, Dongmei. *Proceedings of the 28th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering*. [[Paper](https://doi.org/10.1145/3368089.3409768)]
5. **Efficient bug triage for industrial environments**  
   Zhang, Wei. *2020 IEEE International Conference on Software Maintenance and Evolution (ICSME)*. [[Paper](10.1109/ICSME46990.2020.00082)]
6. **A Method of Component Prediction for Crash Bug Reports Using Component-Based Features and Machine Learning**  
  Xu, Yang and Liu, Chao and Li, Yong and Xie, Qiaoluan and Choi, Hyun-Deok. *2023 IEEE International Conference on Software Analysis, Evolution and Reengineering (SANER)*. [[Paper](https://doi.org/10.1109/SANER56733.2023.00089)]
7. **Knowledge-aware Alert Aggregation in Large-scale Cloud Systems: a Hybrid Approach**  
   Kuang, Jinxi and Liu, Jinyang and Huang, Junjie and Zhong, Renyi and Gu, Jiazhen and Yu, Lan and Tan, Rui and Yang, Zengyin and Lyu, Michael R. *Proceedings of the 46th International Conference on Software Engineering: Software Engineering in Practice*. [[Paper](https://doi.org/10.1145/3639477.3639745)]
8. **X-lifecycle learning for cloud incident management using llms**  
   Goel, Drishti and Husain, Fiza and Singh, Aditya and Ghosh, Supriyo and Parayil, Anjaly and Bansal, Chetan and Zhang, Xuchao and Rajmohan, Saravan. *Companion Proceedings of the 32nd ACM International Conference on the Foundations of Software Engineering*. [[Paper](https://doi.org/10.1145/3663529.3663861)]

#### Social Network Modeling

1. **Reducing bug triaging confusion by learning from mistakes with a bug tossing knowledge graph**  
   Su, Yanqi and Xing, Zhenchang and Peng, Xin and Xia, Xin and Wang, Chong and Xu, Xiwei and Zhu, Liming. *2021 36th IEEE/ACM International Conference on Automated Software Engineering (ASE)*. [[Paper](https://doi.org/10.1109/ASE51524.2021.9678574)]
2. **Still confusing for bug-component triaging? Deep feature learning and ensemble setting to rescue**  
   Su, Yanqi and Han, Zheming and Gao, Zhipeng and Xing, Zhenchang and Lu, Qinghua and Xu, Xiwei. *2023 IEEE/ACM 31st International Conference on Program Comprehension (ICPC)*. [[Paper](https://doi.org/10.1109/ICPC58990.2023.00046)]
3. **Fast outage analysis of large-scale production clouds with service correlation mining**  
   Wang, Yaohui and Li, Guozheng and Wang, Zijian and Kang, Yu and Zhou, Yangfan and Zhang, Hongyu and Gao, Feng and Sun, Jeffrey and Yang, Li and Lee, Pochian and others. *2021 IEEE/ACM 43rd International Conference on Software Engineering (ICSE)*. [[Paper](https://doi.org/10.1109/ICSE43902.2021.00085)]

#### Data Bias Modeling

1. **Learning from evolving data streams: online triage of bug reports**  
   Chrupała, Grzegorz. *Proceedings of the 13th Conference of the European Chapter of the Association for Computational Linguistics*. [[Paper](https://aclanthology.org/E12-1063.pdf)]
2. **Improving it support by enhancing incident management process with multi-modal analysis**  
   Mandal, Atri and Agarwal, Shivali and Malhotra, Nikhil and Sridhara, Giriprasad and Ray, Anupama and Swarup, Daivik. *International Conference on Service-Oriented Computing*. [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-33702-5_33)]
   
### 2.2 Developer Assignment

#### Text Classification

1. **Who Should Fix This Bug?**  
   Anvik, John and Hiew, Lyndon and Murphy, Gail C. *Proceedings of the 28th international conference on Software engineering*. [[Paper](https://www.ifi.uzh.ch/dam/jcr:00000000-2f41-7b40-0000-00005fabb70c/murphy-icse06.pdf)]

2. **Reducing the Effort of Bug Report Triage: Recommenders for Development-Oriented Decisions**  
   Anvik, John and Murphy, Gail C. *ACM Transactions on Software Engineering and Methodology (TOSEM)*. [[Paper](https://dl.acm.org/doi/abs/10.1145/2000791.2000794)]

3. **Automatic Software Bug Triage System (BTS) Based on Latent Semantic Indexing and Support Vector Machine**  
   Ahsan, Syed Nadeem and Ferzund, Javed and Wotawa, Franz. *2009 Fourth International Conference on Software Engineering Advances*. [[Paper](https://dl.acm.org/doi/abs/10.1109/ICSEA.2009.92)]
4. **Automated Bug Assignment: Ensemble-based Machine Learning in Large Scale Industrial Contexts**  
   Jonsson, Leif and Borg, Markus and Broman, David and Sandahl, Kristian and Eldh, Sigrid and Runeson, Per. *Empirical Software Engineering*. [[Paper](https://lucris.lub.lu.se/ws/portalfiles/portal/1859620/7865979.pdf)]
5. **Improving Bug Triaging with High Confidence Predictions at Ericsson**  
   Sarkar, Aindrila and Rigby, Peter C and Bartalos, Bela. *2019 IEEE International Conference on Software Maintenance and Evolution*. [[Paper](https://users.encs.concordia.ca/~pcr/paper/Sarkar2019ICSME.pdf)]
6. **Applying Deep Learning Based Automatic Bug Triager to Industrial Projects**  
   Lee, Sun-Ro and Heo, Min-Jae and Lee, Chan-Gun and Kim, Milhan and Jeong, Gaeul. *Proceedings of the 2017 11th Joint Meeting on foundations of software engineering*. [[Paper](https://dl.acm.org/doi/abs/10.1145/3106237.3117776)]
7. **DeepTriage: Exploring the Effectiveness of Deep Learning for Bug Triaging**  
   Mani, Senthil and Sankaran, Anush and Aralikatte, Rahul. *Proceedings of the ACM India joint international conference on data science and management of data*. [[Paper](https://dl.acm.org/doi/abs/10.1145/3297001.3297023)]
8. **Bug Triaging Based on Tossing Sequence Modeling**  
   Xi, Sheng-Qu and Yao, Yuan and Xiao, Xu-Sheng and Xu, Feng and Lv, Jian. *Journal of Computer Science and Technology*. [[Paper](https://jcst.ict.ac.cn/en/article/pdf/preview/10.1007/s11390-019-1953-5.pdf)]
9. **DeepTriage: Automated Transfer Assistance for Incidents in Cloud Services**  
   Pham, Phuong and Jain, Vivek and Dauterman, Lukas and Ormont, Justin and Jain, Navendu. *Proceedings of the 26th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining*. [[Paper](https://arxiv.org/pdf/2012.03665)]
10. **A Light Bug Triage Framework for Applying Large Pre-trained Language Model**  
   Lee, Jaehyung and Han, Kisun and Yu, Hwanjo. *Proceedings of the 37th IEEE/ACM international conference on automated software engineering*. [[Paper](https://dl.acm.org/doi/abs/10.1145/3551349.3556898)]
11. **An Empirical Assessment of Different Word Embedding and Deep Learning Models for Bug Assignment**  
   Wang, Rongcun and Ji, Xingyu and Xu, Senlei and Tian, Yuan and Jiang, Shujuan and Huang, Rubing. *Journal of Systems and Software*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0164121224000049)]
12. **BTAL: An Imbalance Software Bug Report Triage Approach Based on BERT-TextCNN**  
   Zhang, Yanmei and Sun, Yuhang and Shi, Yi and Jiang, Shujuan and Yuan, Guan. *Information and Software Technology*. [[Paper](https://www.sciencedirect.com/science/article/pii/S0950584925000709)]
13. **Fixer-Level Supervised Contrastive Learning for Bug Assignment**  
   Wang, Rongcun and Ji, Xingyu and Tian, Yuan and Xu, Senlei and Sun, Xiaobing and Jiang, Shujuan. *Empirical Software Engineering*. [[Paper](https://link.springer.com/article/10.1007/s10664-025-10634-0)]   


#### Information Retrieval

1. **Fuzzy Set and Cache-Based Approach for Bug Triaging**  
   Tamrawi, Ahmed and Nguyen, Tung Thanh and Al-Kofahi, Jafar M. and Nguyen, Tien N. *Proceedings of the 19th ACM SIGSOFT Symposium and the 13th European Conference on Foundations of Software Engineering*. [[Paper](https://d1wqtxts1xzle7.cloudfront.net/37152414/viewcontent-libre.pdf?1427685442=&response-content-disposition=inline%3B+filename%3DFuzzy_set_and_cache_based_approach_for_b.pdf&Expires=1762054605&Signature=akkFmk3krfqcn3ySqa93756IGFVuBXH98o6O1joHJfNRF10flY00lt6NaaBnfbL0nLnRKOJ-ywfEW44r9d7lpZ1HolkDHZ87BSSCYflG3MDXgqtS4RqPcun4VanP5s6YtAQemSUgaYtWhCxmQNfsZOy-FCru9QOpaxBviwmxpamLzKBkOD8gh6cl98UMLmzZ1XA0TzJHlAd6mLF4FBa6XUdQ7RmTKYnxaeqRjbva4JvZIJG-D4okkuXM3JcPvsESNepAtkx5JHR8qCTNq7AX47RbF0QWnxrfnuqHqy1ChvlNkzK~OHIpMqtjFBkine4ig4AJr8sFcZtP9JatXOCBfA__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)]

2. **COSTRIAGE: A Cost-Aware Triage Algorithm for Bug Reporting Systems**  
   Park, Jin-woo and Lee, Mu-Woong and Kim, Jinhan and Hwang, Seung-won and Kim, Sunghun. *Proceedings of the AAAI conference on artificial intelligence*. [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/7839)]

3. **Cost-Aware Triage Ranking Algorithms for Bug Reporting Systems**  
   Park, Jin-woo and Lee, Mu-Woong and Kim, Jinhan and Hwang, Seung-won and Kim, Sunghun. *Knowledge and Information Systems*. [[Paper](http://rosaec.snu.ac.kr/meet/file/20120116e.pdf)]
4. **Topic Modeling and Intuitionistic Fuzzy Set-Based Approach for Efficient Software Bug Triaging**  
   Panda, Rama Ranjan and Nagwani, Naresh Kumar. *Knowledge and Information Systems*. [[Paper](https://link.springer.com/article/10.1007/s10115-022-01735-z)]

5. **Vocabulary and Time Based Bug-Assignment: A Recommender System for Open-Source Projects**  
   Sajedi-Badashian, Ali and Stroulia, Eleni. *Software: Practice and Experience*. [[Paper](https://onlinelibrary.wiley.com/doi/abs/10.1002/spe.2830)]
6. **Triaging incoming change requests: Bug or commit history, or code authorship?**   
Mario Linares-Vásquez, Kamal Hossen, Hoang Dang, Huzefa Kagdi, Malcom Gethers, and Denys Poshyvanyk. *IEEE International Conference on Software Maintenance (ICSM)*[[Paper](https://ieeexplore.ieee.org/document/6405306)]
7. **Why So Complicated? Simple Term Filtering and Weighting for Location-Based Bug Report Assignment Recommendation**  
   Shokripour, Ramin and Anvik, John and Kasirun, Zarinah M and Zamani, Sima. *2013 10th working conference on mining software repositories*. [[Paper](https://d1wqtxts1xzle7.cloudfront.net/72977192/msr2013-libre.pdf?1634525411=&response-content-disposition=inline%3B+filename%3DWhy_so_complicated_Simple_term_filtering.pdf&Expires=1762055135&Signature=Yox8ns20-Np5VTlomV7w1b9mlVa27Kq36z41i7Wk1Y73KC1yj8E~K8AlHdvdfqdGFbC2ATuoU2eLRRKKdNLv~cyCfFphoTqcGIRO7Jl6Xqd1-Z6I1OmqGtpgprnFyVKcVmZX1yLVwYnfFQnaXE7PTSEAJ5DUy2rHHWTtJpr~MNgFUUoQgdLxgv4ncnKb8WF0-5cmJTFu0RCgMLgR49D1H9P5tfPXu4iMNgYLHvzIq5pfUh81iofGVvtfbf4s10NSzPrCNBX6lFWqHfAWv0MTOniDXPwp4IRBUGVOJrxBMOEUG4miu4e0evwNkIn70Okr4MyBJpwetiFZKNuD6Wi4aA__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)]
8. **DRETOM: Developer Recommendation Based on Topic Models for Bug Resolution**  
   Xie, Xihao and Zhang, Wen and Yang, Ye and Wang, Qing. *Proceedings of the 8th international conference on predictive models in software engineering*. [[Paper](https://dl.acm.org/doi/abs/10.1145/2365324.2365329)]
9. **Improving Automated Bug Triaging with Specialized Topic Model**  
   Xia, Xin and Lo, David and Ding, Ying and Al-Kofahi, Jafar M. and Nguyen, Tien N. and Wang, Xinyu. *IEEE Transactions on Software Engineering*. [[Paper](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=4693&context=sis_research)]
10. **PorchLight: A Tag-Based Approach to Bug Triaging**  
   Bortis, Gerald and van der Hoek, André. *2013 35th International Conference on Software Engineering*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6606580)]
11. **Towards Semi-automatic Bug Triage and Severity Prediction Based on Topic Model and Multi-feature of Bug Reports**  
   Yang, Geunseok and Zhang, Tao and Lee, Byungjeong. *2014 IEEE 38th Annual Computer Software and Applications Conference*. [[Paper](https://ieeexplore.ieee.org/abstract/document/6899206/)]

#### Social Network Modeling

1. **Improving Bug Triage with Bug Tossing Graphs**  
   Jeong, Gaeul and Kim, Sunghun and Zimmermann, Thomas. *Proceedings of the 7th joint meeting of the European software engineering conference and the ACM SIGSOFT symposium on The foundations of software engineering*. [[Paper](https://research.cs.queensu.ca/home/ahmed/home/teaching/CISC880/F11/papers/BugTossingGraphs_FSE2009.pdf)]

2. **Fine-grained Incremental Learning and Multi-feature Tossing Graphs to Improve Bug Triaging**  
   Bhattacharya, Pamela and Neamtiu, Iulian. *2010 IEEE International Conference on Software Maintenance*. [[Paper](https://www.cs.ucr.edu/~neamtiu/pubs/icsm10bhattacharya.pdf)]

3. **Automated, Highly-Accurate, Bug Assignment Using Machine Learning and Tossing Graphs**  
   Bhattacharya, Pamela and Neamtiu, Iulian and Shelton, Christian R. *Journal of Systems and Software*. [[Paper](https://www.cs.ucr.edu/~neamtiu/pubs/jss12bhattacharya.pdf)]

4. **FixerCache: Unsupervised Caching Active Developers for Diverse Bug Triage**  
   Wang, Song and Zhang, Wen and Wang, Qing. *Proceedings of the 8th ACM/IEEE International Symposium on Empirical Software Engineering and Measurement*. [[Paper](https://www.eecs.yorku.ca/~wangsong/papers/esem14.pdf)]

5. **DECOBA: Utilizing Developers Communities in Bug Assignment**  
   Banitaan, Shadi and Alenezi, Mamdouh. *2013 12th International Conference on Machine Learning and Applications*. [[Paper](https://malenezi.github.io/malenezi/pdfs/DECOBA.pdf)]

6. **Effective bug triage based on historical bug-fix information**  
   Hu, Hao and Zhang, Hongyu and Xuan, Jifeng and Sun, Weigang. *2014 IEEE 25th international symposium on software reliability engineering*. [[Paper](https://doi.org/10.1109/ISSRE.2014.17)]
7. **Enhancing Developer Recommendation with Supplementary Information via Mining Historical Commits**  
   Sun, Xiaobing and Yang, Hui and Xia, Xin and Li, Bin. *Journal of Systems and Software*. [[Paper](https://xin-xia.github.io/publication/jss17.pdf)] 

8. **KSAP: An approach to bug report assignment using KNN search and heterogeneous proximity**  
   Zhang, Wen and Wang, Song and Wang, Qing. *Information and software technology*. [[Paper](https://doi.org/10.1016/j.infsof.2015.10.004)]

9. **A Spatial-Temporal Graph Neural Network Framework for Automated Software Bug Triaging**  
   Wu, Hongrun and Ma, Yutao and Xiang, Zhenglong and Yang, Chen and He, Keqing. *Knowledge-Based Systems*. [[Paper](https://arxiv.org/pdf/2101.11846)]

10. **Graph Collaborative Filtering-Based Bug Triaging**  
   Dai, Jie and Li, Qingshan and Xue, Hui and Luo, Zhao and Wang, Yinglin and Zhan, Siyuan. *Journal of Systems and Software*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0164121223000626)]  

11. **PCG: A Joint Framework of Graph Collaborative Filtering For bug Triaging**  
   Dai, Jie and Li, Qingshan and Xie, Shenglong and Li, Daizhen and Chu, Hua. *Journal of Software: Evolution and Process*. [[Paper](https://onlinelibrary.wiley.com/doi/abs/10.1002/smr.2673)]

12. **Neighborhood Contrastive Learning-based Graph Neural Network for Bug Triaging**  
   Dong, Haozhen and Ren, Hongmin and Shi, Jialiang and Xie, Yichen and Hu, Xudong. *Science of Computer Programming*. [[Paper](https://www.sciencedirect.com/science/article/pii/S0167642324000169?ssrnid=4565134&dgcid=SSRN_redirect_SD)]

13. **Improving Bug Triage with The Bug Personalized Tossing Relationship**  
   Wei, Wei and Li, Haojie and Ren, Xinshuang and Jiang, Feng and Yu, Xu and Gao, Xingyu and Du, Junwei. *Information and Software Technology*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0950584924002477)]

#### Optimization / Decision-Making

1. **T-REC: Towards Accurate Bug Triage for Technical Groups**  
   Pahins, Cicero Augusto De Lara and D'Morison, Fabricio and Rocha, Thiago M and Almeida, Larissa M and Batista, Arthur F and Souza, Diego F. *2019 18th IEEE International Conference on Machine Learning and Applications*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8999225)]

2. **RAPTOR: Release-aware and prioritized bug-fixing task assignment optimization**   
   Yutaro Kashiwa. *IEEE International Conference on Software Maintenance and Evolution (ICSME)*. [[Paper](https://ieeexplore.ieee.org/abstract/document/8919238)]

3. **A Scheduling-Driven Approach to Efficiently Assign Bug Fixing Tasks to Developers**  
   Etemadi, Vahid and Bushehrian, Omid and Akbari, Reza and Robles, Gregorio. *Journal of Systems and Software*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0164121221000649)]

4. **Considering Dependencies Between Bug Reports to Improve Bugs Triage**  
   Almhana, Rafi and Kessentini, Marouane. *Automated Software Engineering*. [[Paper](https://link.springer.com/article/10.1007/s10515-020-00279-2)]   
5. **Wayback Machine: A Tool to Capture The Evolutionary Behavior of The Bug Reports and Their Triage Process in Open-Source Software Systems**  
   Jahanshahi, Hadi and Cevik, Mucahit and Navas-Su, Jose and Basar, Ayse and Gonzalez-Torres, Antonio. *Journal of Systems and Software*. [[Paper](https://arxiv.org/pdf/2011.05382)]
6. **S-DABT: Schedule and Dependency-Aware Bug Triage in Open-Source Bug Tracking Systems**  
   Jahanshahi, Hadi and Cevik, Mucahit. *Information and Software Technology*. [[Paper](https://arxiv.org/pdf/2204.05972)]  

7. **ADPTriage: Approximate Dynamic Programming for Bug Triage**  
   Jahanshahi, Hadi and Cevik, Mucahit and Mousavi, Kianoush and Basar, Ayse. *IEEE Transactions on Software Engineering*. [[Paper](https://arxiv.org/pdf/2211.00872)]  

8. **Navigating Bug Cold Start with Contextual Multi-Armed Bandits: An Enhanced Approach to Developer Assignment in Software Bug Repositories**  
   Singh, Neetu and Singh, Sandeep Kumar. *Automated Software Engineering*. [[Paper](https://link.springer.com/article/10.1007/s10515-025-00508-6)]  

#### Domain-specific Pipelines

1. **WHOSEFAULT: Automatic Developer-to-Fault Assignment through Fault Localization**  
   Servant, Francisco and Jones, James A. *2012 34th International Conference on Software Engineering*. [[Paper](https://fservant.github.io/papers/2012-ICSE.pdf)]  

2. **Towards Intelligent Incident Management: Why We Need It andHow We Make It**  
   Chen, Zhuangbin and Kang, Yu and Li, Liqun and Zhang, Xu and Zhang, Hongyu and Xu, Hui and Zhou, Yangfan and Yang, Li and Sun, Jeffrey and Xu, Zhangwei and Dang, Yingnong and Gao, Feng and Zhao, Pu and Qiao, Bo and Lin, Qingwei and Zhang, Dongmei and Lyu, Michael R. *Proceedings of the 28th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering*. [[Paper](https://netman.aiops.org/~peidan/ANM2023/12.IncidentManagement/zchen_esecfse2020_towards.pdf.pdf)]
3. **Large Language Models Can Provide Accurate and Interpretable Incident Triage**  
   SWang, Zexin and Li, Jianhui and Ma, Minghua and Li, Ze and Kang, Yu and Zhang, Chaoyun and Bansal, Chetan and Chintalapati, Murali and Rajmohan, Saravan and Lin, Qingwei and Zhang, Dongmei and Pei, Changhua and Xie, Gaogang. *2024 IEEE 35th International Symposium on Software Reliability Engineering*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10771420)]

4. **Triangle: Empowering Incident Triage with Multi-LLM-Agents**  
   Yu, Zhaoyang and Ma, Minghua and Feng, Xiaoyu and Ding, Ruomeng and Zhang, Chaoyun and Li, Ze and Chintalapati, Merali and Zhang, Xuchao and Wang, Rujia and Bansal, Chetan and Rajmohan, Sarvan and Lin, Qingwei and Zhang, Shenglin and Pei, Changhua and Pei, Dan. *Proceedings of the 33rd ACM International Conference on the Foundations of Software Engineering*. [[Paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2025/02/TRIANGLE_FSE25.pdf)]


## 3 Feedback and Adaptation

[⬆️top](#table-of-contents)

### 3.1 User Feedback Analysis

1. **Why So Complicated? Simple Term Filtering and Weighting for Location-Based Bug Report Assignment Recommendation**  
   Shokripour, Ramin and Anvik, John and Kasirun, Zarinah M and Zamani, Sima. *2013 10th working conference on mining software repositories*. [[Paper](https://d1wqtxts1xzle7.cloudfront.net/72977192/msr2013-libre.pdf?1634525411=&response-content-disposition=inline%3B+filename%3DWhy_so_complicated_Simple_term_filtering.pdf&Expires=1762012992&Signature=P-QxIvM5H2sA00SBgwcErzsw95tnLOP0wcu3oBNTJjFUgpsKPvLB6iX4B7fTNDMPDetDDc480bPK02iHpjx1TuQRWhLNeWAM~Ok8olt2EGJhAXIj4pxnaLBuelQrubn7JimSLyUtK3c16ruEKK77AitheQ-AUTPrIaPn2ceSr21Y5oO0UmQlEFsxiAttNuhe0KfjSKVbI84pglEB5PuiZQe8oDX8IrOjC3dLRae~YYusFXSAI75J46WXhCa7VoBUlWD3LFV5UgL-~vrywZdHVFprvlQAxW8sY92d-61YJxXEO3V2b5ZiXVTb1lYg9FzkOjsUpl9EmxLwrfHz2jjjcw__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)]

2. **User reviews matter! tracking crowdsourced reviews to support evolution of successful apps**  
   Palomba, Fabio and Linares-Vásquez, Mario and Bavota, Gabriele and Oliveto, Rocco and Di Penta, Massimiliano and Poshyvanyk, Denys and De Lucia, Andrea. *2015 IEEE international conference on software maintenance and evolution (ICSME)*. [[Paper](https://doi.org/10.1109/ICSM.2015.7332475)]

3. **Online App Review Analysis for Identifying Emerging Issues**  
   Gao, Cuiyun and Zeng, Jichuan and Lyu, Michael R and King, Irwin. *Proceedings of the 40th international conference on software engineering*. [[Paper](https://cuiyungao.github.io/publications/cygao_icse2018.pdf)]

4. **Order in Chaos: Prioritizing Mobile App Reviews using Consensus Algorithms**  
   Etaiwi, Layan and Hamel, Sylvie and Gueheneuc, Yann-Gael and Flageol, William and Morales, Rodrigo. *2020 IEEE 44th Annual Computers, Software, and Applications Conference*. [[Paper](https://letaiw.github.io/pubs/COMPSAC2020.pdf)]

5. **Prioritizing User Concerns in App Reviews – A Study of Requests for New Features, Enhancements and Bug Fixes**  
   Malgaonkar, Saurabh and Licorish, Sherlock A and Savarimuthu, Bastin Tony Roy. *Information and Software Technology*. [[Paper](https://dl.acm.org/doi/abs/10.1016/j.infsof.2021.106798)]

6. **Investigating the Criticality of User-Reported Issues Through Their Relations with App Rating**  
   Di Sorbo, Andrea and Grano, Giovanni and Aaron Visaggio, Corrado and Panichella, Sebastiano. *Journal of Software: Evolution and Process*. [[Paper](https://dl.acm.org/doi/abs/10.1002/smr.2316)]

### 3.2 Continuous Triage

1. **Efficient Ticket Routing by Resolution Sequence Mining**  
   Shao, Qihong and Chen, Yi and Tao, Shu and Yan, Xifeng and Anerousis, Nikos. *Proceedings of the 14th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*. [[Paper](https://web.njit.edu/~ychen/publications/sigkdd08_ticket.pdf)]

2. **Continuous Incident Triage for Large-Scale Online Service Systems**  
   Chen, Junjie and He, Xiaoting and Lin, Qingwei and Zhang, Hongyu and Hao, Dan and Gao, Feng and Xu, Zhangwei and Dang, Yingnong and Zhang, Dongmei. *2019 34th IEEE/ACM International Conference on Automated Software Engineering (ASE)*. [[Paper](https://netman.aiops.org/~peidan/ANM2019/12.IncidentManagement/LectureCoverage/2019ASE_Continuous%20Incident%20Triage%20for%20Large-Scale%20Online%20Service%20Systems.pdf)]

3. **Scouts: Improving the Diagnosis Process Through Domain-customized Incident Routing**  
   Gao, Jiaqi and Yaseen, Nofel and MacDavid, Robert and Frujeri, Felipe Vieira and Liu, Vincent and Bianchini, Ricardo and Aditya, Ramaswamy and Wang, Xiaohang and Lee, Henry and Maltz, David, and Yu Minlan, and Arzani Behnaz. *Proceedings of the Annual conference of the ACM Special Interest Group on Data Communication on the applications, technologies, architectures, and protocols for computer communication*. [[Paper](https://dl.acm.org/doi/abs/10.1145/3387514.3405867)]

4. **Ticket-BERT: Labeling Incident Management Tickets with Language Models**  
   Liu, Zhexiong and Benge, Cris and Jiang, Siduo. *arXiv preprint arXiv:2307.00108*. [[Paper](https://arxiv.org/pdf/2307.00108)]
   
5. **Triangle: Empowering Incident Triage with Multi-LLM-Agents**  
   Yu, Zhaoyang and Ma, Minghua and Feng, Xiaoyu and Ding, Ruomeng and Zhang, Chaoyun and Li, Ze and Chintalapati, Merali and Zhang, Xuchao and Wang, Rujia and Bansal, Chetan and Rajmohan, Sarvan and Lin, Qingwei and Zhang, Shenglin and Pei, Changhua and Pei, Dan. *Proceedings of the 33rd ACM International Conference on the Foundations of Software Engineering*. [[Paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2025/02/TRIANGLE_FSE25.pdf)]

6. **An Agentic Framework for Triaging Incidents in Production Cloud Infrastructure**   
   Yuhan Yao, Yuxuan Jiang, Minghua Ma, Vaidya Madhura, Jieren Deng, Yigong Hu, Bansal Chetan, Ze Li, and Chintalapati Murali. *Companion Proceedings of the 34th ACM International Conference on the Foundations of Software Engineering*[[Paper](https://conf.researchr.org/details/fse-2026/fse-2026-industry-papers/27/An-Agentic-Framework-for-Triaging-Incidents-in-Production-Cloud-Infrastructure)]

