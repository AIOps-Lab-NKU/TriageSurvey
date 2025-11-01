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
