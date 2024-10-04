# **오픈소스SW개발론**

### Introduction

-------------
### Week1-1 강의 개요 (강의계획서)
* 교과목명: 오픈소스 소프트웨어 **(SAI0003-2)**
  
* 이 과목은 3가지 목표를 지향한다.
> 오픈소스 소프트웨어 개발을 위한 기본 개념과 도구, 특히 **소스 코드 버전 컨트롤**과 패키지 관리, 프로젝트 빌드를 중점으로 배운다.

> **애자일 기반** 소프트웨어 개발 방법인 짝 프로그래밍, 테스트 주도 개발, 행위 주도 개발, 클라우드 기반 데브옵스를 공부한다.

> 새로운/낯선 소프트웨어 개발 환경 및 도구를 **스스로 배우는 태도**를 배우는 것을 목적으로 한다.  

* 평가비율

![과제1](https://github.com/user-attachments/assets/5c2a9775-5591-4551-980e-e8c9745fbb3f)

- 시험일정
  
     * 중간고사: 7주차
     * 기말고사: 15주차

> [강의 영상](https://www.youtube.com/playlist?list=PLhbaMvGyp999F4RqSqCoXetq8OcT1IfJW)

-------------
### Week1-2 오픈소스소프트웨어 개요 [(강의자료)](https://docs.google.com/presentation/d/1HJM_NecZ2YZMin9NEL7-_PbZnj44ahYD/edit#slide=id.p1)

### **1. github octoverse**

* [The state of open source software](https://octoverse.github.com/)

### **2. What is _Open Source Software_?**

> 소프트웨어 저작권 소유자가 모든 사람에게 소스 코드를 **게시, 사용, 복사, 수정 및 배포할 권리**를 부여한 소프트웨어
* ### **2-1. Commercial SW**
  * 개별 이용허락
  * 로열티 지급
  * 실행 바이너리만 제공
  * 복제, 배포, 수정 불가
  * 사용 기간과 목적 제한

* ### **2-2. Open Source SW**
  * 일괄 사전 이용허락
  * 로열티 없음
  * 소스 코드 제공
  * 복제, 배포, 수정 허용
  * 기간/목적 제한 없음

### **3. Free Software vs. Open Source Software**

* ### **3-1. Free Software**
  ![aaaa](https://github.com/user-attachments/assets/978dbbf0-5e0d-4214-8fe6-5bd8545d8c6a)
  * Richard Stallman – Creator of GNU Project
  * FSF (Free Software Foundation, 1984~)
    * GPL 1.0 (1989), GPL 2.0 (1991), GPL 3.0 (2007)
  * Copyleft  (No SW patent, No DRM)

* ### **3-2. Open Source Software**
  ![bbbb](https://github.com/user-attachments/assets/b4fa2eb6-2b25-4f61-8201-6448b604f959)
  * Eric S. Raymond – Author of 'The Cathedral and the Bazzar (성당과 시장)'
  * OSI (Open Source Initiative, 1998~)
    * Ambiguity of `free’
    * Combination of OSS and Closed Source SW
    * License under law

### **4. Open Source Software Lisence**

> 오픈소스 소프트웨어의 **사용, 복제, 수정, 배포 권한의 범위**를 지정

![cccc](https://github.com/user-attachments/assets/bb557a62-db69-4dff-bab6-eafa1e315f9d)


-------------
### Week2-1 버전 관리 개요 [(강의자료)](https://docs.google.com/presentation/d/1y_XxFORFUVf5NVa40FTFmv9MemetVjBj/edit#slide=id.p1)

### **1. Version Control System (VCS)**
* Track your files over time so that you can easily get back to a previous working version
* VCS software
   * CVS (Concurrent Version System)
   * SVN (Subversion)
   * Mercurial
   * Darcs
   * Git
* Repository or Repo (저장소)

### **2. General Actions in VCS**
* ### **2-1. Checkin**
  ![image](https://github.com/user-attachments/assets/b40eb8f2-ae78-44aa-a1e2-35ab9a8e533d)
  * Check in a file and modify it over time
* ### **2-2. Checkout and editing**
  ![image](https://github.com/user-attachments/assets/92079481-d0e8-4408-8622-150742122122)
  * Check out, edit, and check in a file
* ### **2-3. Diffs**
  ![image](https://github.com/user-attachments/assets/5644d908-a9b2-499b-be2a-f2e058541858)
  * The trunk has a history of changes as a file evolves
* ### **2-4. Branching**
  ![image](https://github.com/user-attachments/assets/dd9f1bca-01d2-4806-8be1-26464ac99560)
  * Copy code into a separate folder so we can have a separate history of changes
* ### **2-5. Merging**
  ![image](https://github.com/user-attachments/assets/49ade0d9-5f12-4d20-8c76-b7a6ceef570b)
  * Merge changes from one branch to another
* ### **2-6. Conflicts**
  ![image](https://github.com/user-attachments/assets/f8159876-d81e-4a49-a668-e5e327359c24)
  * When changes overlap like an example below
* ### **2-7. Tagging**
  ![image](https://github.com/user-attachments/assets/df38de9d-cca5-4bb5-bb7c-3e29079c7ad8)
  * Let you tag (label) any revision for easy reference

### **3. Two Main Types of VCS**
* ### **3-1. Centralized VCS**
  * One central repository with many users
     * Ex) CVS, SVN, Darcs
* ### **3-2. Decentralized (Distributed) VCS**
  * Every user owns his or her local repository
  * A separate remote (central) repository
    * Sometimes, more than one remote (central) repositories

  * Two new actions (with remote repositories): fork pull request
    * Ex) GIT, Mercurial
 

-------------
### Week2-2 Git [(강의자료)](https://docs.google.com/presentation/d/1y_XxFORFUVf5NVa40FTFmv9MemetVjBj/edit#slide=id.p1)
### **1. Introduction to GIT**
![image](https://github.com/user-attachments/assets/474b5eca-8033-43cd-8693-3f96cb2a75cb)
* Linus Torvalds
   * For collaboration of development of Linux kernel
* A distributed version control system
   * Workspace : files you are working with
   * Index: (staged) files to be considered in the next commit
   * Local repository : files committed to the local repo
   * Remote repository : files pushed to the remote repo
### **2. GIT Workflow**
![image](https://github.com/user-attachments/assets/cadd69f3-3cb2-4dbf-a0c6-a5bb0b33b9a6)

-------------
### Week2-3 Github, fork, pull request
### **1. GITHUB**
> [깃허브 링크](https://github.com/)

> Git-based Source Code Hosting for Social Coding

### **2. Fork** [(참고한 자료)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project.html#_forking_projects)
![image](https://github.com/user-attachments/assets/7f3f7d87-3c6f-41d8-96db-6f6470676074)


 > If you want to contribute to an existing project to which you don’t have push access, you can “fork” the project

 > the same project in your own namespace, allowing you to make changes
   to a project publicly as a way to contribute in a more open manner

### **3. Pull Request**
* 다른프로젝트에 내가 만든 commit을 제출한다는 의미
   * 실제 전송단위는 branch
* fork한 github 프로젝트를 토대로 새로운 commit 내용들을 제출 가능


[My Github Blog](https://github.com/MYEYEYE)

-------------
### Week2-4 Git: Advanced topics
### **1. merge로 2개 브랜치 합치기**
 * git checkout 현재브랜치명
 * git merge 합칠 브랜치명

### **2. rebase**
> 한 브랜치에서 변경된 사항을 다른 브랜치에 적용 가능

### **3. 중간에 낀 commmit 수정하기**
  * git rebase -i --root
  * git commit --ammend -sm "커밋 메시지"
  * git rebase --continue

### **4. blame으로 추적하기**
  * git blame 파일명
  * git show 커밋아이디

-------------
### Week3: Markdown [(실습링크)]()
### **1. 이탤릭체와 볼드체**
* 이탤릭체: 문장 처음과 끝에 '_' 붙여서 사용
   * ex) _a_ , _b_
* 볼드체: 문장 처음과 끝에 '**' 붙여서 사용
   * ex) **a**, **b**
* 둘이 동시 적용도 가능
   * ex) **_a_**, **_b_**

### **2. 헤더**
* 문장의 앞에 ‘#’ 붙여서 사용
* #을 1개부터 6개까지 추가해 사용 가능
   * 많이 추가할수록 글씨의 크기 감소
* 제목, 부제를 나타낼 때 사용

### **3. 링크**
* 인라인 링크
   "[텍스트] (링크주소)" 
* 참조 링크
   * "[태그][참조]"
   * "[참조]: 링크"

### **4. 이미지**
* 맨 앞에 ! 붙여줘야함 (나머지는 링크와 동일)

### **5. 인용문**
* 문장 앞에 > 추가해 사용
  > 인용

### **6. 리스트**
* 순서가 있는 리스트
   * 순서대로 1. 2. 3. ... 붙여서 사용
* 순서가 없는 리스트
   * *붙여서 사용
   * 공백 개수로 세부단계 구분

### **7. 단락 나눔**
* 개행 나눔
   * 개행으로 단락 구분
* 줄 나눔
   * 문장의 끝에서 스페이스 2번 눌러 구분
  

