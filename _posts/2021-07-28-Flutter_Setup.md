---
title: "[Flutter] 플러터와 안드로이드 스튜디오 다운로드 방법"
date: 2021-5-9
categories:
  - study
tags:
  - flutter
toc: true
toc_ads: true
toc_sticky: true
---

<br>
<br>

## 1. Flutter 다운받기


![2](https://user-images.githubusercontent.com/46369038/127249845-2181b3b9-b354-49cf-818a-d56e39bd9aa7.png)


https://flutter.dev/docs/get-started/install


본인 운영체제에 맞는 flutter 버전 다운 받기


![3](https://user-images.githubusercontent.com/46369038/127249846-67d47b02-f5cd-4acb-8e57-07bd1a317609.png)


다운 받은 폴더 압축을 풀고, 'flutter'폴더를 루트 폴더인 'C 드라이브'로 이동시키기

<br>
<br>

## 2. Git 다운로드


![7](https://user-images.githubusercontent.com/46369038/127249855-7bd106a9-752e-44c7-8179-b50439facede.png)


http://git-scm.com/download/ 에서 운영체제에 맞는 Git 다운로드


기본값으로 다 next 선택해서 다운로드하면 끝

<br>
<br>

## 3. 환경 변수 설정하기


![5](https://user-images.githubusercontent.com/46369038/127249849-274fcb7d-502e-406c-925e-f29513e49d4f.png)


Windows 설정 제어판 > 시스템 > 정보 > 시스템 정보 클릭 > 고급 시스템 설정 > 환경 변수에서 설정


![6](https://user-images.githubusercontent.com/46369038/127249852-7af8aa22-3fb2-4239-bd18-bc5761ee13a9.png)


만약 Path변수가 없으면, '새로 만들기'를 누르고 아래와 같이 입력


- 변수 이름 'Path'
- 변수 값 : 'C:\flutter\bin' (앞에 flutter 폴더 주소 + bin)


만약 Path 변수가 이미 있으면 선택 후 '편집' > '새로만들기' > 'C:\flutter\bin' 입력 > 확인

<br>
<br>

## 4. 환경 변수 설정 확인하기


![8](https://user-images.githubusercontent.com/46369038/127249856-807637d0-baa9-451a-8046-97dcc07e054d.png)


Windows Powershell > 'flutter' 입력 후 위와 같이 나오면 잘 성정된 것


만약 오류나면 환경변수 설정이 잘못된 것이므로 위에서 다시 설정해야함

<br>
<br>

## 5. Android Studio 설치하기


![9](https://user-images.githubusercontent.com/46369038/127249858-fced21f1-4022-412c-be5c-c3458446bd4e.png)


https://d.android.com/studio 에서 안드 스튜디오 다운로드 후 기본값으로 다 next 선택


![10](https://user-images.githubusercontent.com/46369038/127249860-a09baff4-7c3e-4621-80dc-8468aeff159b.png)


완료되면 안드로이드 스튜디오 자동 시작


불러들여올 파일이 있으면 'config or installation folder', 없으면 'do not import settings' 클릭


data sharing할건지 묻는 창이 뜨는데, 답변과 상관없이 프로그램 다운 받을 수 있으므로 아무거나


이후 창에서 기본값으로 다 next 누르고 다운로드하면 끝

<br>
<br>

## 6. Android Studio에 Flutter 플러그인 설치하기


![11](https://user-images.githubusercontent.com/46369038/127249862-1e85d9ce-46cd-49b7-9c88-36c90f794ea8.png)


웰컴 창에서 plug 탭을 누른다


![12](https://user-images.githubusercontent.com/46369038/127249863-f14d3b1b-5e20-4032-88f2-c63567e2061a.png)


'flutter' 검색해서 다운로드하는데 중간에 알림창 나오는데 다 yes


plugin이 정상적으로 설치되어 있으면 welcomscreen에 create new flutter project라고 뜸

<br>
<br>

## 7. Android Studio Emulator 설정하기


![13](https://user-images.githubusercontent.com/46369038/127249866-60538c3d-cd68-4f57-970c-7d9ae04c8e69.png)


웰컴 창에서 AVD Manager 탭을 누른다


![15](https://user-images.githubusercontent.com/46369038/127249872-abcc0d61-4143-4f82-ade0-778a44e462d4.png)


설정창이 뜨면 'Create Virtual Device'를 선택


Select Hardware에서 원하는 카테고리 설정


저는 앱용 어플을 주로 만들어서 Phone을 클릭하고 Playstore가 있는 Pixel4로 주로 설치함


![16](https://user-images.githubusercontent.com/46369038/127249875-5250aee2-bd1e-4547-82e6-b4fcdad4f71b.png)


시스템 이미지는 보통 R로 선택하면 자동 다운로드되지는데


다운로드가 다 되면 이미지 선택이 가능해짐


이미지 선택후 다음 누르고 또 다음 누르면 에뮬레이터 선택 가능


![17](https://user-images.githubusercontent.com/46369038/127249838-6ebbc304-be8d-4d70-988d-61b93f9b371c.png)


그러면 에뮬레이터에 해당 기기가 나오는데 ▶ 이 버튼 누르면 구동이 됨

<br>
<br>

## 8. Dart SDK is not configured 해결법


![20](https://user-images.githubusercontent.com/46369038/127249844-7ab7eb51-91a3-4838-aeeb-dc157c140baa.png)


다운로드가 다 완료되서 창을 열면 'Dart SDK is not configured'이라는 문구가 뜬다


해결책은 상단에 File > Setting > Languages & Frameworks > Flutter에서


Flutter SDK path에 다운 받은 Flutter 폴더를 선택해주면 된다

<br>
<br>

## 9. Java_home 설정해주기


![22](https://user-images.githubusercontent.com/46369038/127254329-824cbb7e-a420-4b7b-b7a1-24e10405b042.png)


설치가 되면 'pubspec.yaml' 파일을 클릭하고 들어가서 오른쪽 상단의 Flutter Doctor를 클릭하면 현재 설치 상황이 나온다


근데 처음 설치하니 2번째가 에러가 떴는데


Java_home 어쩌구하면서 Path 설정이 안되었다는 오류가 났다


![23](https://user-images.githubusercontent.com/46369038/127254803-b722cd24-6039-4ac7-bf24-873fdd10d2ca.png)


https://www.oracle.com/java/technologies/javase-downloads.html


그러면 위에 주소로 들어가서 JDK Download를 클릭해서 다운 받는다


다운받을때 기본값으로 다음 누르고 다운받으면 되는데, 다만 인스톨 되는 주소는 외우고 있어야 한다


보통 기본 주소로 'C:\Program Files\Java' 안에다가 다운 되는 듯


![24](https://user-images.githubusercontent.com/46369038/127255245-77162684-dea2-46a9-84b3-bce123c963f8.png)


다운로드가 다 되면 jdk가 설치된 경로를 들어가서 주소복사를 해놓고


환경변수 > 시스템 변수 > 새로 만들기를 눌러 복사한 주소를 붙여넣기하고 확인을 누르면 끝

<br>
<br>

## 10. Chocolatey 다운받기


![25](https://user-images.githubusercontent.com/46369038/127255645-8113ad9d-afa4-4227-a137-86380ecabe80.png)


https://chocolatey.org/install


위에 가서 다운로드 명령어 주소 복사


![26](https://user-images.githubusercontent.com/46369038/127255781-35917564-d7f0-4b1b-b028-1e805fbf3bc8.png)


Window shell을 관리자 권한으로 실행


![18](https://user-images.githubusercontent.com/46369038/127249841-8e50b5bd-d95f-44ac-bccf-1e918307cb0a.png)


위에서 복사한 주소를 붙여넣어주면 위와 같은 화면이 나오고 끝

<br>
<br>
