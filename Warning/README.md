# Paper deatils and data desription

## 1) WarningsGuru: Integrating Statistical Bug Models with Static Analysis to Provide Timely and Specific Bug Warnings:
The detection of bugs in software systems has been divided into two research areas: static code analysis and statistical modeling of historical data. Static analysis indicates precise problems on line numbers but has the disadvantage of suggesting many warning which are often false positives. In contrast, statistical models use the history of the system to suggest which files or commits are likely to contain bugs. These course-grained predictions do not indicate to the developer the precise reasons for the bug prediction. We com- bine static analysis with statistical bug models to limit the number of warnings and provide specific warnings information at the line level. Previous research was able to process only a limited number of releases, our tool, WarningsGuru, can analyze all commits in a source code repository and we currently have processed thou- sands of commits and warnings. Since we process every commit, we present developers with more precise information about when a warning is introduced allowing us to show recent warnings that are introduced in statistically risky commits. Results from two OSS projects show that CommitGuru’s statistical model flags 25% and 29% of all commits as risky. When we combine this with static analy- sis in WarningsGuru the number of risky commits with warnings is 20% for both projects and the number commits with new warnings is only 3% and 6%. We can drastically reduce the number of commits and warnings developers have to examine. The tool, source code, and demo is available at https://github.com/louisq/warningsguru.

* somewhat similar to commit guru but for static warning

Datasets: Not specifically mentioned