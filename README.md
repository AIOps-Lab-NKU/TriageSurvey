# TriageSurvey
A Survey of Triage in Software Engineering

## Triage Lifecycle
Triage encompasses a sequence of analytical activities aimed at efficiently managing the lifecycle of an issue. The process involves identifying duplicates, prioritizing the issue's urgency, classifying the issue's type, and routing the issue to the most appropriate entity for resolution. This entity may be a specific developer, a component team, or an automated analysis pipeline. ![](assets/overall.png)

## Table of Contents
- [Datasets](#datasets)
- [Toolkits](#toolkits)
- [0 Data Processing](#0-data-processing)
  - [0.1 Deduplication](#01-deduplication)
  - [0.2 Feature Extraction](#02-feature-extraction)
- [1 Prioritization](#1-prioritization)
  - [1.1 Severity Rating](#11-severity-rating)
  - [1.2 Issue Type Classification](#12-issue-type-classification)
- [2 Assignment](2-assignment)
  - [2.1 Component Assignment](21-component-assignment)
  - [2.2 Developer Assignment](22-developer-assignment)
- [3 Postmortem Process](3-postmortem-process)
  - [3.1 Continuous Triage](31-continuous-triage)
  - [3.2 User Feedback Analysis](32-user-feedback-analysis)
 
## Datasets
1. **MultiTriage**: Bug reports from Eclipse & Github OSS projects. [[Source](https://github.com/thazin31086/MultiTriage/tree/master/Project/Data)]


## Toolkits

## 0 Data Processing

[**⬆️top**](#table-of-contents)

### 0.1 Deduplication

#### Incident Reports

1. **Mining Historical Issue Repositories to Heal Large-Scale Online Service Systems**  
   Ding, Rui and Fu, Qiang and Lou, Jian Guang and Lin, Qingwei and Zhang, Dongmei and Xie, Tao. *2014 44th Annual IEEE/IFIP International Conference on Dependable Systems and Networks*. [[Paper](https://netman.aiops.org/~peidan/ANM2018Fall/6.LogAnomalyDetection/ReadingList/Mining%20Historical%20Issue%20Repositories%20to%20Heal%20Large-Scale%20Online%20Service%20Systems.pdf)]

#### Bug Reports

#### Alerts

#### Reviews


### 0.2 Feature Extraction

#### Incident Reports

#### Bug Reports

#### Observability Data

#### Reviews

#### Relational Data


## 1 Prioritization

[⬆️top](#table-of-contents)

### 1.1 Severity Rating

### 1.2 Issue Type Classification


## 2 Assignment

[⬆️top](#table-of-contents)

### 2.1 Component Assignment

### 2.2 Developer Assignment

#### Text Classification

1. **Who Should Fix This Bug?**  
   Anvik, John and Hiew, Lyndon and Murphy, Gail C. *Proceedings of the 28th international conference on Software engineering*. [[Paper](https://www.ifi.uzh.ch/dam/jcr:00000000-2f41-7b40-0000-00005fabb70c/murphy-icse06.pdf)]

2. **Reducing the Effort of Bug Report Triage: Recommenders for Development-Oriented Decisions**  
   Anvik, John and Murphy, Gail C. *ACM Transactions on Software Engineering and Methodology (TOSEM)*. [[Paper](https://dl.acm.org/doi/abs/10.1145/2000791.2000794)]

3. **Automatic Software Bug Triage System (BTS) Based on Latent Semantic Indexing and Support Vector Machine**  
   Ahsan, Syed Nadeem and Ferzund, Javed and Wotawa, Franz. *2009 Fourth International Conference on Software Engineering Advances*. [[Paper](https://dl.acm.org/doi/abs/10.1109/ICSEA.2009.92)]

4. **COSTRIAGE: A Cost-Aware Triage Algorithm for Bug Reporting Systems**  
   Park, Jin-woo and Lee, Mu-Woong and Kim, Jinhan and Hwang, Seung-won and Kim, Sunghun. *Proceedings of the AAAI conference on artificial intelligence*. [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/7839)]

5. **Applying Deep Learning Based Automatic Bug Triager to Industrial Projects**  
   Lee, Sun-Ro and Heo, Min-Jae and Lee, Chan-Gun and Kim, Milhan and Jeong, Gaeul. *Proceedings of the 2017 11th Joint Meeting on foundations of software engineering*. [[Paper](https://dl.acm.org/doi/abs/10.1145/3106237.3117776)]

6. **DeepTriage: Exploring the Effectiveness of Deep Learning for Bug Triaging**  
   Mani, Senthil and Sankaran, Anush and Aralikatte, Rahul. *Proceedings of the ACM India joint international conference on data science and management of data*. [[Paper](https://dl.acm.org/doi/abs/10.1145/3297001.3297023)]

7. **Bug Triaging Based on Tossing Sequence Modeling**  
   Xi, Sheng-Qu and Yao, Yuan and Xiao, Xu-Sheng and Xu, Feng and Lv, Jian. *Journal of Computer Science and Technology*. [[Paper](https://jcst.ict.ac.cn/en/article/pdf/preview/10.1007/s11390-019-1953-5.pdf)]

8. **A Light Bug Triage Framework for Applying Large Pre-trained Language Model**  
   Lee, Jaehyung and Han, Kisun and Yu, Hwanjo. *Proceedings of the 37th IEEE/ACM international conference on automated software engineering*. [[Paper](https://dl.acm.org/doi/abs/10.1145/3551349.3556898)]

9. **An Empirical Assessment of Different Word Embedding and Deep Learning Models for Bug Assignment**  
   Wang, Rongcun and Ji, Xingyu and Xu, Senlei and Tian, Yuan and Jiang, Shujuan and Huang, Rubing. *Journal of Systems and Software*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0164121224000049)]

10. **An Ensemble Method for Bug Triaging using Large Language Models**  
   Kumar Dipongkor, Atish. *Proceedings of the 2024 IEEE/ACM 46th International Conference on Software Engineering: Companion Proceedings*. [[Paper](https://dl.acm.org/doi/abs/10.1145/3639478.3641228)]

11. **Cost-Aware Triage Ranking Algorithms for Bug Reporting Systems**  
   Park, Jin-woo and Lee, Mu-Woong and Kim, Jinhan and Hwang, Seung-won and Kim, Sunghun. *Knowledge and Information Systems*. [[Paper](http://rosaec.snu.ac.kr/meet/file/20120116e.pdf)]

12. **Automated Bug Assignment: Ensemble-based Machine Learning in Large Scale Industrial Contexts**  
   Jonsson, Leif and Borg, Markus and Broman, David and Sandahl, Kristian and Eldh, Sigrid and Runeson, Per. *Empirical Software Engineering*. [[Paper](https://lucris.lub.lu.se/ws/portalfiles/portal/1859620/7865979.pdf)]

13. **Improving Bug Triaging with High Confidence Predictions at Ericsson**  
   Sarkar, Aindrila and Rigby, Peter C and Bartalos, Bela. *2019 IEEE International Conference on Software Maintenance and Evolution*. [[Paper](https://users.encs.concordia.ca/~pcr/paper/Sarkar2019ICSME.pdf)]

14. **BTAL: An Imbalance Software Bug Report Triage Approach Based on BERT-TextCNN**  
   Zhang, Yanmei and Sun, Yuhang and Shi, Yi and Jiang, Shujuan and Yuan, Guan. *Information and Software Technology*. [[Paper](https://www.sciencedirect.com/science/article/pii/S0950584925000709)]

15. **Fixer-Level Supervised Contrastive Learning for Bug Assignment**  
   Wang, Rongcun and Ji, Xingyu and Tian, Yuan and Xu, Senlei and Sun, Xiaobing and Jiang, Shujuan. *Empirical Software Engineering*. [[Paper](https://link.springer.com/article/10.1007/s10664-025-10634-0)]

#### Information Retrieval

1. **Fuzzy Set and Cache-Based Approach for Bug Triaging**  
   Tamrawi, Ahmed and Nguyen, Tung Thanh and Al-Kofahi, Jafar M. and Nguyen, Tien N. *Proceedings of the 19th ACM SIGSOFT Symposium and the 13th European Conference on Foundations of Software Engineering*. [[Paper](https://d1wqtxts1xzle7.cloudfront.net/37152414/viewcontent-libre.pdf?1427685442=&response-content-disposition=inline%3B+filename%3DFuzzy_set_and_cache_based_approach_for_b.pdf&Expires=1762054605&Signature=akkFmk3krfqcn3ySqa93756IGFVuBXH98o6O1joHJfNRF10flY00lt6NaaBnfbL0nLnRKOJ-ywfEW44r9d7lpZ1HolkDHZ87BSSCYflG3MDXgqtS4RqPcun4VanP5s6YtAQemSUgaYtWhCxmQNfsZOy-FCru9QOpaxBviwmxpamLzKBkOD8gh6cl98UMLmzZ1XA0TzJHlAd6mLF4FBa6XUdQ7RmTKYnxaeqRjbva4JvZIJG-D4okkuXM3JcPvsESNepAtkx5JHR8qCTNq7AX47RbF0QWnxrfnuqHqy1ChvlNkzK~OHIpMqtjFBkine4ig4AJr8sFcZtP9JatXOCBfA__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)]

2. **Topic Modeling and Intuitionistic Fuzzy Set-Based Approach for Efficient Software Bug Triaging**  
   Panda, Rama Ranjan and Nagwani, Naresh Kumar. *Knowledge and Information Systems*. [[Paper](https://link.springer.com/article/10.1007/s10115-022-01735-z)]

3. **Vocabulary and Time Based Bug-Assignment: A Recommender System for Open-Source Projects**  
   Sajedi-Badashian, Ali and Stroulia, Eleni. *Software: Practice and Experience*. [[Paper](https://onlinelibrary.wiley.com/doi/abs/10.1002/spe.2830)]

4. **Effective Bug Triage for Non-Reproducible Bugs**  
   Goyal, Anjali. *2017 IEEE/ACM 39th International Conference on Software Engineering Companion*. [[Paper](https://ieeexplore.ieee.org/abstract/document/7965397)]

5. **Triaging Incoming Change Requests: Bug or Commit History, or Code Authorship?**  
   Linares-Vásquez, Mario and Hossen, Kamal and Dang, Hoang and Kagdi, Huzefa and Gethers, Malcom and Poshyvanyk, Denys. *2012 28th IEEE International Conference on Software Maintenance*. [[Paper](https://www.cs.wm.edu/~denys/pubs/ICSM'12-DevRecAuthorship.pdf)]

6. **Why So Complicated? Simple Term Filtering and Weighting for Location-Based Bug Report Assignment Recommendation**  
   Shokripour, Ramin and Anvik, John and Kasirun, Zarinah M and Zamani, Sima. *2013 10th working conference on mining software repositories*. [[Paper](https://d1wqtxts1xzle7.cloudfront.net/72977192/msr2013-libre.pdf?1634525411=&response-content-disposition=inline%3B+filename%3DWhy_so_complicated_Simple_term_filtering.pdf&Expires=1762055135&Signature=Yox8ns20-Np5VTlomV7w1b9mlVa27Kq36z41i7Wk1Y73KC1yj8E~K8AlHdvdfqdGFbC2ATuoU2eLRRKKdNLv~cyCfFphoTqcGIRO7Jl6Xqd1-Z6I1OmqGtpgprnFyVKcVmZX1yLVwYnfFQnaXE7PTSEAJ5DUy2rHHWTtJpr~MNgFUUoQgdLxgv4ncnKb8WF0-5cmJTFu0RCgMLgR49D1H9P5tfPXu4iMNgYLHvzIq5pfUh81iofGVvtfbf4s10NSzPrCNBX6lFWqHfAWv0MTOniDXPwp4IRBUGVOJrxBMOEUG4miu4e0evwNkIn70Okr4MyBJpwetiFZKNuD6Wi4aA__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)]

7. **DRETOM: Developer Recommendation Based on Topic Models for Bug Resolution**  
   Xie, Xihao and Zhang, Wen and Yang, Ye and Wang, Qing. *Proceedings of the 8th international conference on predictive models in software engineering*. [[Paper](https://dl.acm.org/doi/abs/10.1145/2365324.2365329)]

8. **Effective Bug Triage based on Historical Bug-Fix Information**  
   Hu, Hao and Zhang, Hongyu and Xuan, Jifeng and Sun, Weigang. *2014 IEEE 25th international symposium on software reliability engineering*. [[Paper](https://inria.hal.science/hal-01087444/file/140831_BugFixer_ISSRE_1811.pdf)]

9. **Improving Automated Bug Triaging with Specialized Topic Model**  
   Xia, Xin and Lo, David and Ding, Ying and Al-Kofahi, Jafar M. and Nguyen, Tien N. and Wang, Xinyu. *IEEE Transactions on Software Engineering*. [[Paper](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=4693&context=sis_research)]

10. **PorchLight: A Tag-Based Approach to Bug Triaging**  
   Bortis, Gerald and van der Hoek, André. *2013 35th International Conference on Software Engineering*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6606580)]

#### Social Network Modeling

1. **Improving Bug Triage with Bug Tossing Graphs**  
   Jeong, Gaeul and Kim, Sunghun and Zimmermann, Thomas. *Proceedings of the 7th joint meeting of the European software engineering conference and the ACM SIGSOFT symposium on The foundations of software engineering*. [[Paper](https://research.cs.queensu.ca/home/ahmed/home/teaching/CISC880/F11/papers/BugTossingGraphs_FSE2009.pdf)]

2. **Automated, Highly-Accurate, Bug Assignment Using Machine Learning and Tossing Graphs**  
   Bhattacharya, Pamela and Neamtiu, Iulian and Shelton, Christian R. *Journal of Systems and Software*. [[Paper](https://www.cs.ucr.edu/~neamtiu/pubs/jss12bhattacharya.pdf)]

3. **FixerCache: Unsupervised Caching Active Developers for Diverse Bug Triage**  
   Wang, Song and Zhang, Wen and Wang, Qing. *Proceedings of the 8th ACM/IEEE International Symposium on Empirical Software Engineering and Measurement*. [[Paper](https://www.eecs.yorku.ca/~wangsong/papers/esem14.pdf)]

4. **DECOBA: Utilizing Developers Communities in Bug Assignment**  
   Banitaan, Shadi and Alenezi, Mamdouh. *2013 12th International Conference on Machine Learning and Applications*. [[Paper](https://malenezi.github.io/malenezi/pdfs/DECOBA.pdf)]

5. **A Spatial-Temporal Graph Neural Network Framework for Automated Software Bug Triaging**  
   Wu, Hongrun and Ma, Yutao and Xiang, Zhenglong and Yang, Chen and He, Keqing. *Knowledge-Based Systems*. [[Paper](https://arxiv.org/pdf/2101.11846)]

6. **PCG: A Joint Framework of Graph Collaborative Filtering For bug Triaging**  
   Dai, Jie and Li, Qingshan and Xie, Shenglong and Li, Daizhen and Chu, Hua. *Journal of Software: Evolution and Process*. [[Paper](https://onlinelibrary.wiley.com/doi/abs/10.1002/smr.2673)]

6. **Neighborhood Contrastive Learning based Graph Neural Network for Bug Triaging**  
   Dong, Haozhen and Ren, Hongmin and Shi, Jialiang and Xie, Yichen and Hu, Xudong. *Science of Computer Programming*. [[Paper](https://www.sciencedirect.com/science/article/pii/S0167642324000169?ssrnid=4565134&dgcid=SSRN_redirect_SD)]

#### Optimization / Decision-Making

1. **A Bug You Like: A Framework for Automated Assignment of Bugs**  
   Baysal, Olga and Godfrey, Michael W and Cohen, Robin. *2009 IEEE 17th International Conference on Program Comprehension*. [[Paper](https://plg.uwaterloo.ca/~migod/papers/2009/icpc09-olga-longVersion.pdf)]

2. **T-REC: Towards Accurate Bug Triage for Technical Groups**  
   Pahins, Cicero Augusto De Lara and D'Morison, Fabricio and Rocha, Thiago M and Almeida, Larissa M and Batista, Arthur F and Souza, Diego F. *2019 18th IEEE International Conference on Machine Learning and Applications*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8999225)]

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

9. **Triangle: Empowering Incident Triage with Multi-LLM-Agents**  
   Yu, Zhaoyang and Ma, Minghua and Feng, Xiaoyu and Ding, Ruomeng and Zhang, Chaoyun and Li, Ze and Chintalapati, Merali and Zhang, Xuchao and Wang, Rujia and Bansal, Chetan and Rajmohan, Sarvan and Lin, Qingwei and Zhang, Shenglin and Pei, Changhua and Pei, Dan. *Proceedings of the 33rd ACM International Conference on the Foundations of Software Engineering*. [[Paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2025/02/TRIANGLE_FSE25.pdf)]

#### Other / Hybrid

1. **WHOSEFAULT: Automatic Developer-to-Fault Assignment through Fault Localization**  
   Servant, Francisco and Jones, James A. *2012 34th International Conference on Software Engineering*. [[Paper](https://fservant.github.io/papers/2012-ICSE.pdf)]  

2. **DeCaf: Diagnosing and Triaging Performance Issues in Large-Scale Cloud Services**  
   Bansal, Chetan and Renganathan, Sundararajan and Asudani, Ashima and Midy, Olivier and Janakiraman, Mathru. *Proceedings of the ACM/IEEE 42nd International Conference on Software Engineering: Software Engineering in Practice*. [[Paper](https://arxiv.org/pdf/1910.05339)]  

3. **Identifying Recurrent and Unknown Performance Issues**  
   Lim, Meng-Hui and Lou, Jian-Guang and Zhang, Hongyu and Fu, Qiang and Teoh, Andrew Beng Jin and Lin, Qingwei and Ding, Rui and Zhang, Dongmei. *2014 IEEE International Conference on Data Mining*. [[Paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/07/ICDM2014-Identifying-Recurrent-and-Unknown-Performance-Issues.pdf)]  

4. **Towards Semi-automatic Bug Triage and Severity Prediction Based on Topic Model and Multi-feature of Bug Reports**  
   Yang, Geunseok and Zhang, Tao and Lee, Byungjeong. *2014 IEEE 38th Annual Computer Software and Applications Conference*. [[Paper](https://ieeexplore.ieee.org/abstract/document/6899206/)]

5. **Fine-grained Incremental Learning and Multi-feature Tossing Graphs to Improve Bug Triaging**  
   Bhattacharya, Pamela and Neamtiu, Iulian. *2010 IEEE International Conference on Software Maintenance*. [[Paper](https://www.cs.ucr.edu/~neamtiu/pubs/icsm10bhattacharya.pdf)]

6. **KSAP: An Approach to Bug Report Assignment using KNN Search and Heterogeneous Proximity**  
   Zhang, Wen and Wang, Song and Wang, Qing. *Information and software technology*. [[Paper](https://www.eecs.yorku.ca/~wangsong/papers/ist16.pdf)]

7. **DeepTriage: Automated Transfer Assistance for Incidents in Cloud Services**  
   Pham, Phuong and Jain, Vivek and Dauterman, Lukas and Ormont, Justin and Jain, Navendu. *Proceedings of the 26th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining*. [[Paper](https://arxiv.org/pdf/2012.03665)]

8. **Towards Intelligent Incident Management: Why We Need It andHow We Make It**  
   Chen, Zhuangbin and Kang, Yu and Li, Liqun and Zhang, Xu and Zhang, Hongyu and Xu, Hui and Zhou, Yangfan and Yang, Li and Sun, Jeffrey and Xu, Zhangwei and Dang, Yingnong and Gao, Feng and Zhao, Pu and Qiao, Bo and Lin, Qingwei and Zhang, Dongmei and Lyu, Michael R. *Proceedings of the 28th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering*. [[Paper](https://netman.aiops.org/~peidan/ANM2023/12.IncidentManagement/zchen_esecfse2020_towards.pdf.pdf)]
 
9. **Graph Collaborative Filtering-Based Bug Triaging**  
   Dai, Jie and Li, Qingshan and Xue, Hui and Luo, Zhao and Wang, Yinglin and Zhan, Siyuan. *Journal of Systems and Software*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0164121223000626)]  

10. **Enhancing Developer Recommendation with Supplementary Information via Mining Historical Commits**  
   Sun, Xiaobing and Yang, Hui and Xia, Xin and Li, Bin. *Journal of Systems and Software*. [[Paper](https://xin-xia.github.io/publication/jss17.pdf)]  

11. **Large Language Models Can Provide Accurate and Interpretable Incident Triage**  
   SWang, Zexin and Li, Jianhui and Ma, Minghua and Li, Ze and Kang, Yu and Zhang, Chaoyun and Bansal, Chetan and Chintalapati, Murali and Rajmohan, Saravan and Lin, Qingwei and Zhang, Dongmei and Pei, Changhua and Xie, Gaogang. *2024 IEEE 35th International Symposium on Software Reliability Engineering*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10771420)]

12. **Improving Bug Triage with The Bug Personalized Tossing Relationship**  
   Wei, Wei and Li, Haojie and Ren, Xinshuang and Jiang, Feng and Yu, Xu and Gao, Xingyu and Du, Junwei. *Information and Software Technology*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0950584924002477)]


## 3 Postmortem Process

[⬆️top](#table-of-contents)

### 3.1 Continuous Triage

1. **Continuous Incident Triage for Large-Scale Online Service Systems**  
   Chen, Junjie and He, Xiaoting and Lin, Qingwei and Zhang, Hongyu and Hao, Dan and Gao, Feng and Xu, Zhangwei and Dang, Yingnong and Zhang, Dongmei. *2019 34th IEEE/ACM International Conference on Automated Software Engineering (ASE)*. [[Paper](https://netman.aiops.org/~peidan/ANM2019/12.IncidentManagement/LectureCoverage/2019ASE_Continuous%20Incident%20Triage%20for%20Large-Scale%20Online%20Service%20Systems.pdf)]

2. **Efficient Ticket Routing by Resolution Sequence Mining**  
   Shao, Qihong and Chen, Yi and Tao, Shu and Yan, Xifeng and Anerousis, Nikos. *Proceedings of the 14th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*. [[Paper](https://web.njit.edu/~ychen/publications/sigkdd08_ticket.pdf)]

3. **Scouts: Improving the Diagnosis Process Through Domain-customized Incident Routing**  
   Gao, Jiaqi and Yaseen, Nofel and MacDavid, Robert and Frujeri, Felipe Vieira and Liu, Vincent and Bianchini, Ricardo and Aditya, Ramaswamy and Wang, Xiaohang and Lee, Henry and Maltz, David, and Yu Minlan, and Arzani Behnaz. *Proceedings of the Annual conference of the ACM Special Interest Group on Data Communication on the applications, technologies, architectures, and protocols for computer communication*. [[Paper](https://dl.acm.org/doi/abs/10.1145/3387514.3405867)]

4. **Ticket-BERT: Labeling Incident Management Tickets with Language Models**  
   Liu, Zhexiong and Benge, Cris and Jiang, Siduo. *arXiv preprint arXiv:2307.00108*. [[Paper](https://arxiv.org/pdf/2307.00108)]
   
5. **Triangle: Empowering Incident Triage with Multi-LLM-Agents**  
   Yu, Zhaoyang and Ma, Minghua and Feng, Xiaoyu and Ding, Ruomeng and Zhang, Chaoyun and Li, Ze and Chintalapati, Merali and Zhang, Xuchao and Wang, Rujia and Bansal, Chetan and Rajmohan, Sarvan and Lin, Qingwei and Zhang, Shenglin and Pei, Changhua and Pei, Dan. *Proceedings of the 33rd ACM International Conference on the Foundations of Software Engineering*. [[Paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2025/02/TRIANGLE_FSE25.pdf)]

### 3.2 User Feedback Analysis

1. **Why So Complicated? Simple Term Filtering and Weighting for Location-Based Bug Report Assignment Recommendation**  
   Shokripour, Ramin and Anvik, John and Kasirun, Zarinah M and Zamani, Sima. *2013 10th working conference on mining software repositories*. [[Paper](https://d1wqtxts1xzle7.cloudfront.net/72977192/msr2013-libre.pdf?1634525411=&response-content-disposition=inline%3B+filename%3DWhy_so_complicated_Simple_term_filtering.pdf&Expires=1762012992&Signature=P-QxIvM5H2sA00SBgwcErzsw95tnLOP0wcu3oBNTJjFUgpsKPvLB6iX4B7fTNDMPDetDDc480bPK02iHpjx1TuQRWhLNeWAM~Ok8olt2EGJhAXIj4pxnaLBuelQrubn7JimSLyUtK3c16ruEKK77AitheQ-AUTPrIaPn2ceSr21Y5oO0UmQlEFsxiAttNuhe0KfjSKVbI84pglEB5PuiZQe8oDX8IrOjC3dLRae~YYusFXSAI75J46WXhCa7VoBUlWD3LFV5UgL-~vrywZdHVFprvlQAxW8sY92d-61YJxXEO3V2b5ZiXVTb1lYg9FzkOjsUpl9EmxLwrfHz2jjjcw__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)]

2. **User Reviews Matter! Tracking Crowdsourced Reviews to Support Evolution of Successful Apps**  
   Palomba, Fabio and Linares-V{\'a}squez, Mario and Bavota, Gabriele and Oliveto, Rocco and Di Penta, Massimiliano and Poshyvanyk, Denys and De Lucia, Andrea. *2015 IEEE international conference on software maintenance and evolution*. [[Paper](https://s3.eu-central-1.amazonaws.com/eu-st01.ext.exlibrisgroup.com/39UBZ_INST/storage/alma/EA/E4/37/7F/72/CF/BC/22/3A/A6/92/07/53/31/D0/DB/Pal-Lin-Bav-Oli-DiP-Pos-DeL_UserReviewsMatter.pdf?response-content-type=application%2Fpdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20251101T150515Z&X-Amz-SignedHeaders=host&X-Amz-Expires=119&X-Amz-Credential=AKIAJN6NPMNGJALPPWAQ%2F20251101%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Signature=7b249aa3466f34bf8473383d628f76a183f68683224242edd94d4c0abafcba3c)]

3. **Online App Review Analysis for Identifying Emerging Issues**  
   Gao, Cuiyun and Zeng, Jichuan and Lyu, Michael R and King, Irwin. *Proceedings of the 40th international conference on software engineering*. [[Paper](https://cuiyungao.github.io/publications/cygao_icse2018.pdf)]

4. **Order in Chaos: Prioritizing Mobile App Reviews using Consensus Algorithms**  
   Etaiwi, Layan and Hamel, Sylvie and Gueheneuc, Yann-Gael and Flageol, William and Morales, Rodrigo. *2020 IEEE 44th Annual Computers, Software, and Applications Conference*. [[Paper](https://letaiw.github.io/pubs/COMPSAC2020.pdf)]

5. **Prioritizing User Concerns in App Reviews – A Study of Requests for New Features, Enhancements and Bug Fixes**  
   Malgaonkar, Saurabh and Licorish, Sherlock A and Savarimuthu, Bastin Tony Roy. *Information and Software Technology*. [[Paper](https://dl.acm.org/doi/abs/10.1016/j.infsof.2021.106798)]

6. **Investigating the Criticality of User-Reported Issues Through Their Relations with App Rating**  
   Di Sorbo, Andrea and Grano, Giovanni and Aaron Visaggio, Corrado and Panichella, Sebastiano. *Journal of Software: Evolution and Process*. [[Paper](https://dl.acm.org/doi/abs/10.1002/smr.2316)]
