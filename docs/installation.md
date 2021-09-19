# Smart Mandate
## Release Status
[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=paycorp-io_smart-mandate&metric=ncloc&token=c77c80860cc7302cf80a90c11d1a798e206688f1)](https://sonarcloud.io/dashboard?id=paycorp-io_smart-mandate)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=paycorp-io_smart-mandate&metric=bugs&token=c77c80860cc7302cf80a90c11d1a798e206688f1)](https://sonarcloud.io/dashboard?id=paycorp-io_smart-mandate)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=paycorp-io_smart-mandate&metric=sqale_rating&token=c77c80860cc7302cf80a90c11d1a798e206688f1)](https://sonarcloud.io/dashboard?id=paycorp-io_smart-mandate)
[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=paycorp-io_smart-mandate&metric=code_smells&token=c77c80860cc7302cf80a90c11d1a798e206688f1)](https://sonarcloud.io/dashboard?id=paycorp-io_smart-mandate)

## smart-mandate Description
Mandate solutions for Paycorp.io



##Steps to give release :
***********************

1) git clone https://github.com/paycorp-io/smart-mandate.git PAYCORP-RELEASE

2) cd PAYCORP-RELEASE
**********************************
Delete the existing release  branch to  avoid conflicts
To delete the branch → git branch -d release → locally
To delete the branch remotely →  git push origin --delete release → remotely
**********************************
3) git checkout -b release

4) git push origin release

5) cd smart-mandate

6) mvn clean install

7) mvn external.atlassian.jgitflow:jgitflow-maven-plugin:release-start -DautoVersionSubmodules=true -Dmaven.javadoc.skip=true

8) mvn external.atlassian.jgitflow:jgitflow-maven-plugin:release-finish -DautoVersionSubmodules=true -Dmaven.javadoc.skip=true

9) cd ..

10) git push origin release

11) git push origin master

12) git push --tags

To push Release to Nexus

13)if you are in release branch  do git checkout release

14)mvn deploy
