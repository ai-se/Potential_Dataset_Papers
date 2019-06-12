# Paper deatils and data desription

## 1) MORE: A Multi-objective Refactoring Recommendation Approach to Introducing Design Patterns and Fixing Code Smells:
Refactoring is widely recognized as a crucial technique applied when evolving object-oriented software systems. If applied well, refactoring can improve different aspects of software quality including readability, maintainability and extendibility. However, despite its importance and benefits, recent studies report that automated refactoring tools are underused much of the time by software developers. This paper introduces an automated approach for refactoring recommendation, called MORE, driven by three objectives: (1) to improve design quality (as defined by software quality metrics), (2) to fix code smells, and (3) to introduce design patterns. To this end, we adopt the recent non-dominated sorting genetic algorithm, NSGA-III, to find the best trade-off between these three objectives. We evaluated the efficacy of our approach using a benchmark of seven medium and large open-source systems, seven commonly-occurring code smells (god class, feature envy, data class, spaghetti code, shotgun surgery, lazy class, and long parameter list), and four common design pattern types (visitor, factory method, singleton and strategy). Our approach is empirically evaluated through a quantitative and qualitative study to compare it against three different state-of-the art approaches, two popular multi-objective search algorithms, as well as random search. The statistical analysis of the results confirms the efficacy of our approach in improving the quality of the studied systems while successfully fixing 84% of code smells and introducing an average of six design patterns. In addition, the qualitative evaluation shows that most of the suggested refactorings (an average of 69%) are considered by developers to be relevant and meaningful.

* uses quality metrices to define and find code smells

Datasets: 7 projects

## 2) An experimental investigation on the innate relationship between quality and refactoring:
Previous studies have investigated the reasons behind refactoring operations performed by developers, and proposed methods and tools to recommend refactorings based on quality metric profiles, or on the presence of poor design and implementation choices, i.e., code smells. Nevertheless, the existing literature lacks obser- vations about the relations between metrics/code smells and refactoring activities performed by developers. In other words, the characteristics of code components increasing/decreasing their chances of being object of refactoring operations are still unknown. This paper aims at bridging this gap. Specifically, we mined the evolution history of three Java open source projects to investigate whether refactoring activities occur on code components for which certain indicators—such as quality metrics or the presence of smells as detected by tools—suggest there might be need for refactoring operations. Results indicate that, more often than not, quality metrics do not show a clear relationship with refactoring. In other words, refactoring operations are generally focused on code components for which quality metrics do not suggest there might be need for refactoring operations. Finally, 42% of refactoring operations are performed on code entities affected by code smells. However, only 7% of the performed operations actually remove the code smells from the affected class.

* shows quality metrices doesn't always represents refactoring and code smells properly.

Datasets: 3 Java projects

## 3) An expert system for determining candidate software classes for refactoring:
In the lifetime of a software product, development costs are only the tip of the iceberg. Nearly 90% of the cost is maintenance due to error correction, adaptation and mainly enhancements. As Lehman and Belady [Lehman, M. M., & Belady, L. A. (1985). Program evolution: Processes of software change. Academic Press Professional.] state that software will become increasingly unstructured as it is changed. One way to overcome this problem is refactoring. Refactoring is an approach which reduces the software complexity by incrementally improving internal software quality. Our motivation in this research is to detect the classes that need to be rafactored by analyzing the code complexity. We propose a machine learning based model to predict classes to be refactored. We use Weighted Naïve Bayes with InfoGain heuristic as the learner and we conducted experiments with metric data that we collected from the largest GSM operator in Turkey. Our results showed that we can predict 82% of the classes that need refactoring with 13% of manual inspection effort on the average.

* shows the need of certain type of refactoring on classes can be detected using ML

Datasets: 1 Project

## 4) Constructing models for predicting extract subclass refactoring opportunities using object-oriented quality metrics:
Refactoring is a maintenance task that refers to the process of restructuring software source code to enhance its quality without affecting its external behavior. Inspecting and analyzing the source code of the system under consideration to identify the classes in need of extract subclass refactoring (ESR) is a time consuming and costly process.
Objective: This paper explores the abilities of several quality metrics considered individually and in com- bination to predict the classes in need of ESR.
For a given a class, this paper empirically investigates, using univariate logistic regression anal- ysis, the abilities of 25 existing size, cohesion, and coupling metrics to predict whether the class is in need of restructuring by extracting a subclass from it. In addition, models of combined metrics based on mul- tivariate logistic regression analysis were constructed and validated to predict the classes in need of ESR, and the best model is justifiably recommended. We explored the statistical relations between the values of the selected metrics and the decisions of the developers of six open source Java systems with respect to whether the classes require ESR.
Results: The results indicate that there was a strong statistical relation between some of the quality met- rics and the decision of whether ESR activity was required. From a statistical point of view, the recom- mended model of metrics has practical thresholds that lead to an outstanding classification of the classes into those that require ESR and those that do not.
The proposed model can be applied to automatically predict the classes in need of ESR and present them as suggestions to developers working to enhance the system during the maintenance phase. In addition, the model is capable of ranking the classes of the system under consideration according to their degree of need of ESR.

* shows extract subclass refactoring can be detected using LR(univarient and multivarient) with different quality metrices.

Datasets: 6 Projects

## 5) Empirical evaluation of software maintainability based on a manually validated refactoring dataset:
Context: Refactoring is a technique for improving the internal structure of software systems. It has a solid theoretical background while being used in development practice also. However, we lack empirical research results on the real effect of code refactoring and its application.
Objective: This paper presents a manually validated subset of a previously published dataset containing the refactorings extracted by the RefFinder tool, code metrics, and maintainability of 7 open-source systems. We found that RefFinder had around 27% overall average precision on the subject systems, thus our manually validated subset has substantial added value. Using the dataset, we studied several aspects of the refactored and non-refactored source code elements (classes and methods), like the differences in their maintainability and source code metrics.
Method: We divided the source code elements into a group containing the refactored elements and a group with non-refactored elements. We analyzed the elements’ characteristics in these groups using correlation analysis, Mann–Whitney U test and effect size measures.
Results: Source code elements subjected to refactorings had significantly lower maintainability than elements not affected by refactorings. Moreover, refactored elements had significantly higher size related metrics, com- plexity, and coupling. Also these metrics changed more significantly in the refactored elements. The results are mostly in line with our previous findings on the not validated dataset, with the difference that clone metrics had no strong connection with refactoring.
Conclusions: Compared to the preliminary analysis using a not validated dataset, the manually validated dataset led to more significant results, which suggests that developers find targets for refactorings based on some in- ternal quality properties of the source code, like their size, complexity or coupling, but not clone related metrics as reported in our previous studies. They do not just use these properties for identifying targets, but also control them with refactorings.

* uses maintainability index to see if refactoring affects maintainability index.

Datasets: 7 OSS projects

## 6) Identifying Extract Method Refactoring Opportunities Based on Functional Relevance:
‘Extract Method’ is considered one of the most frequently applied and beneficial refactorings, since the corresponding Long Method smell is among the most common and persistent ones. Although Long Method is conceptually related to the implementation of diverse functionalities within a method, until now, this relationship has not been utilized while identifying refactoring opportunities. In this paper we introduce an approach (accompanied by a tool) that aims at identifying source code chunks that collaborate to provide a specific functionality, and propose their extraction as separate methods. The accuracy of the proposed approach has been empirically validated both in an industrial and an open-source setting. In the former case, the approach was capable of identifying functionally related statements within two industrial long methods (approx. 500 LoC each), with a recall rate of 93 percent. In the latter case, based on a comparative study on open-source data, our approach ranks better compared to two well-known techniques of the literature. To assist software engineers in the prioritization of the suggested refactoring opportunities the approach ranks them based on an estimate of their fitness for extraction. The provided ranking has been validated in both settings and proved to be strongly correlated with experts’ opinion.

* uses code analysis using AST to identify potential candidates for extract method refactoring.

Datasets: 1 Industry partner's dataset.

## 7) Predicting Classes in Need of Refactoring: An Application of Static Metrics:
This paper introduces a class-based approach to predicting refactoring candidates. Using a selected set of static metrics and a weighted ranking method, a tool was designed to predict a prioritized list of classes in need of refactoring. A study was designed and undertaken to compare the performance of the refactoring decision tool to that of human reviewers on the task of finding design problems that reduce class maintainability. The study results indicate that such a refactoring decision support tool can greatly assist the software team. The study also provided useful information on how to augment the functionalities of the refactoring tool.

* uses OO metrices to predict classes need of refactoring

Datasets: Not clarified

## 8) Predicting move method refactoring opportunities in object-oriented code:
Context: Refactoring is the maintenance process of restructuring software source code to improve its quality without changing its external behavior. Move Method Refactoring (MMR) refers to moving a method from one class to the class in which the method is used the most often. Manually inspecting and analyzing the source code of the system under consideration to determine the methods in need of MMR is a costly and time-consuming process. Existing techniques for identifying MMR opportunities have several limitations, such as scalability problems and being inapplicable in early development stages. Most of these techniques do not consider semantic relationships.
Objective: We introduce a measure and a corresponding model to precisely predict whether a class includes methods in need of MMR. The measure is applicable once a class has entered the early devel- opment stages without waiting for other classes to be developed.
Method: The proposed measure considers both the cohesion and coupling aspects of methods. In ad- dition, the measure uses structural and semantic data available within the class of interest. A statistical technique is applied to construct prediction models for classes that include methods in need of MMR. The models are applied on seven object-oriented systems to empirically evaluate their abilities to predict MMR opportunities.
Results: The results show both that the prediction models based on the proposed measure had outstand- ing prediction abilities and that the measure was able to correctly detect more than 90% of the methods in need of MMR within the predicted classes.
Conclusions: The proposed measure and corresponding prediction models are expected to greatly assist software engineers both in locating classes that include methods in need of MMR and in identifying these methods within the predicted classes.

* uses few hybrid metrices(obtained from OO metrices; though not all are CK metrices) to predict for move method refactoring opportunities

Datasets: 7 projects

## 9) Rank-based refactoring decision support: two studies:
Refactoring can result in code with improved maintainability and is considered a preventive maintenance activity. Managers of large projects need ways to decide where to apply scarce resources when performing refactor- ing. There is a lack of tools for supporting such decisions. We introduce a rank-based software measure-driven refac- toring decision support approach to assist managers. The approach uses various static measures to develop a weighted rank, ranking classes or packages that need refactoring. We undertook two case studies to examine the effectiveness of the approach. Specifically, we wanted to see if the decision support tool yielded results similar to those of human ana- lysts/managers and in less time so that it can be used to aug- ment human decision making. In the first study, we found that our approach identified classes as needing refactoring that were also identified by humans. In the second study, a hierarchical approach was used to identify packages that had actually been refactored in 15 releases of the open source project Tomcat. We examined the overlap between the tool’s findings and the actual refactoring activities. The tool reached 100/86.7% recall on the package/class level. Though these studies were limited in size and scope, it appears that this approach is worthy of further examination.

* uses static measures to identify and rank classes need of refactoring

Datasets: 1 Project

## 10) Towards Just-In-Time Refactoring Recommenders:
Empirical studies have provided ample evidence that low code quality is generally associated with lower maintainability. For this reason, tools have been developed to automatically detect design flaws (e.g., code smells). However, these tools are not able to prevent the introduction of design flaws. This means that the code has to experience a quality decay (with a consequent increase of mainte- nance/evolution costs) before state-of-the-art tools can be applied to identify and refactor the design flaws.
Our goal is to develop a new generation of refactoring recom- menders aimed at preventing, via refactoring operations, the intro- duction of design flaws rather than fixing them once they already affect the system. We refer to such a novel perspective on software refactoring as just-in-time refactoring. In this paper, we make a first step towards this direction, presenting an approach able to predict which classes will be affected in the future by code smells.

* JIT refactoring detctor by using COSP (COde Smell Predictor). Which in turn using OO metrices to find code smells in code.

Datasets: 6 Projects

## 11) Understanding the Impact of Refactoring on Smells: A Longitudinal Study of 23 Software Projects:
Code smells in a program represent indications of structural quality problems, which can be addressed by software refactoring. However, refactoring intends to achieve different goals in practice, and its application may not reduce smelly structures. Developers may neglect or end up creating new code smells through refactoring. Unfortunately, little has been reported about the beneficial and harmful effects of refactoring on code smells. This paper reports a longitudinal study intended to address this gap. We analyze how often commonly-used refactoring types affect the density of 13 types of code smells along the version histories of 23 projects. Our findings are based on the analysis of 16,566 refactorings distributed in 10 different types. Even though 79.4% of the refactorings touched smelly elements, 57% did not reduce their occurrences. Surprisingly, only 9.7% of refactorings removed smells, while 33.3% induced the introduction of new ones. More than 95% of such refactoring- induced smells were not removed in successive commits, which suggest refactorings tend to more frequently introduce long-living smells instead of eliminating existing ones. We also characterized and quantified typical refactoring-smell patterns, and observed that harmful patterns are frequent, including: (i) approximately 30% of the Move Method and Pull Up Method refactorings induced the emergence of God Class, and (ii) the Extract Superclass refactoring creates the smell Speculative Generality in 68% of the cases.

* uses various methods to identify effect of refactoring on code smells and are the refactorinf operations are performed on smelly codes.

Datasets: 23 projects

## 12) Accurate and Efficient Refactoring Detection in Commit History:
Refactoring detection algorithms have been crucial to a variety of applications: (i) empirical studies about the evolution of code, tests, and faults, (ii) tools for library API migration, (iii) improving the comprehension of changes and code reviews, etc. However, recent research has questioned the accuracy of the state-of-the-art refactoring detection tools, which poses threats to the reliability of their application. Moreover, previous refactoring detection tools are very sensitive to user-provided similarity thresholds, which further reduces their practical accuracy. In addition, their requirement to build the project versions/revisions under analysis makes them inapplicable in many real-world scenarios.
To reinvigorate a previously fruitful line of research that has sti- fled, we designed, implemented, and evaluated RMiner, a technique that overcomes the above limitations. At the heart of RMiner is an AST-based statement matching algorithm that determines refac- toring candidates without requiring user-defined thresholds. To empirically evaluate RMiner, we created the most comprehensive oracle to date that uses triangulation to create a dataset with con- siderably reduced bias, representing 3,188 refactorings from 185 open-source projects. Using this oracle, we found that RMiner has a precision of 98% and recall of 87%, which is a significant improvement over the previous state-of-the-art.

* This is the refactorminer tool that we have used for identifying java refactoring

Datasets: 185 Projects

## 13) The Buggy Side of Code Refactoring: Understanding the Relationship between Refactorings and Bugs:
Code refactoring is widely practiced by software developers. There is an explicit assumption that code refactoring improves the struc- tural quality of a software project, thereby also reducing its bug proneness. However, refactoring is often applied with different purposes in practice. Depending on the complexity of certain refac- torings, developers might unconsciously make the source code more susceptible to have bugs. In this paper, we present a longitudi- nal study of 5 Java open source projects, where 20,689 refactorings, and 1,033 bug reports were analyzed. We found that many bugs are introduced in the refactored code as soon as the first immedi- ate change is made on it. Furthermore, code elements affected by refactorings performed in conjunction with other changes are more prone to have bugs than those affected by pure refactorings.

* This paper/poster tries to show if refactoring introduces bugs

Datasets: 5 Projects

## 14) Identifying refactoring opportunities in object-oriented code: A systematic literature review:
Context: Identifying refactoring opportunities in object-oriented code is an important stage that precedes the actual refactoring process. Several techniques have been proposed in the literature to identify oppor- tunities for various refactoring activities.
Objective: This paper provides a systematic literature review of existing studies identifying opportunities for code refactoring activities.
Method: We performed an automatic search of the relevant digital libraries for potentially relevant stud- ies published through the end of 2013, performed pilot and author-based searches, and selected 47 pri- mary studies (PSs) based on inclusion and exclusion criteria. The PSs were analyzed based on a number of criteria, including the refactoring activities, the approaches to refactoring opportunity identification, the empirical evaluation approaches, and the data sets used.
Results: The results indicate that research in the area of identifying refactoring opportunities is highly active. Most of the studies have been performed by academic researchers using nonindustrial data sets. Extract Class and Move Method were found to be the most frequently considered refactoring activities. The results show that researchers use six primary existing approaches to identify refactoring opportuni- ties and six approaches to empirically evaluate the identification techniques. Most of the systems used in the evaluation process were open-source, which helps to make the studies repeatable. However, a rela- tively high percentage of the data sets used in the empirical evaluations were small, which limits the gen- erality of the results.
Conclusions: It would be beneficial to perform further studies that consider more refactoring activities, involve researchers from industry, and use large-scale and industrial-based systems.

* A literature review paper for all types of refactoring papers

Datasets: NA

## 15) A New Design Defects Classification: Marrying Detection and Correction:
Previous work classify design defects based on symptoms (long methods, large classes, long parameter lists, etc.), and treat separately detection and correction steps. This paper introduces a new classification of defects using correction possibilities. Thus, correcting different code fragments appending to specific defect category need, approximately, the same refactoring operations to apply. To this end, we use genetic programming to generate new form of classification rules combining detection and correction steps. We report the results of our validation using different open-source systems. Our proposal achieved high precision and recall correction scores.

* classifies classes need of refactoring using rule based genetic mutation.

Datasets: 6 Projects

## 16) Refactoring - Improving Coupling and Cohesion of Existing Code:
Refactorings are widely recognised as ways to improve the internal structure of object-oriented software while maintaining its external behaviour. Unfortunately, refac- torings concentrate on the treatment of symptoms (the so called code-smells), thus improvements depend a lot on the skills of the maintainer. Coupling and cohesion on the other hand are quality attributes which are generally recognized as being among the most likely quantifiable indicators for software maintainability. Therefore, this paper analyzes how refactorings manipulate coupling/cohesion character- istics, and how to identify refactoring opportunities that im- prove these characteristics. As such we provide practical guidelines for the optimal usage of refactoring in a software maintenance process.

* shows the effect of different refactoring operation on cohesion and coupling

Datasets: NA


## 17) Revisiting the Relationship Between Code Smells and Refactoring:
Refactoring is a critical technique in evolving soft- ware systems. Martin Fowler presented a catalogue of refactoring patterns that defines a list of code smells and their corresponding refactoring patterns. This list aimed at supporting programmers in finding suitable refactoring patterns that remove code smells from their systems. However, a recent empirical study by Bavota et al. shows that refactoring rarely removes code smells which do not align with Fowler’s catalog. To bridge the gap between them, we revisit the relationship between code smells and refactorings. In this study, we investigate whether developers apply appropriate refactoring patterns to fix code smells in three open source software systems.

* shows relationship between code smells and refactoring operations

Datasets: 3 projects

## 18) Improving Code Maintainability: A Case Study on the Impact of Refactoring:
It is a fact that a lot of software is written by people without a formal education in software engineering. As an example, material scientists often capture their knowledge in the form of simulation software that contains sophisticated al- gorithms representing complex physical concepts. Since software engineering is typically not a core skill of these scientists, there is a risk that their software becomes unmaintainable once it reaches a substantial size or structural complexity.
This paper reports on a case study in which software engineers consulted magnetics researchers in refactoring their simulation software. This software had grown to 30 kloc of Java and was considered unmaintainable by the stakeholders of the research project. The case study describes the process of refactoring a system under the guidance of a software engineer with results supported by static analysis and software metrics. It shows how software engineers evaluated and selected refactorings to apply to the system using their expert judgment with input from static analysis tools and discusses the outcome of refactoring as evaluated by code owners and reported via static analysis metrics.

*  shows how refactoring improves code maintainability in one case study

Datasets: 1 Project

## 19) Method Level Refactoring Prediction on Five Open Source Java Projects using Machine Learning Techniques:
Introduction : Identifying code segments in large and complex systems in need of refactoring is non-trivial for software devel- opers. Our research aim is to develop recommendation systems for suggesting methods which require refactoring. Materials and Methods : Previous research shows that source code metrics for object-oriented software systems are indicators of complexity of a software system. We compute 25 different source code metrics at the method level and use it as features in a machine learning framework to predict the need of refactoring. We conduct a series of experiments on a publicly available annotated dataset of five software systems to investigate the performance of our proposed approach. In this proposed solution, ten different machine learning classifiers have been considered. In order to handle issues related to class imbalance, three different data sampling methods are also considered during implementation. Conclusion : Our analysis re- veals that the mean accuracy for the SMOTE and RUSBoost data sampling technique is 98.47% respectively. The mean accuracy for the classifier AdaBoost is 98.16% and the mean accuracy for the classifier ANN+GD is 98.17% respectively. Hypothesis testing re- sults reveals that the performance of different classifiers and data sampling techniques are statistically significant in nature.

* 
