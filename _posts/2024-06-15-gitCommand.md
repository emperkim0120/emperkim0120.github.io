---
layout: single
title: "자주 사용하는 Git 명령어"
categories: coding
toc: true
author_profile: false
sidebar:
    nav: "docs"
---



4) 자주 사용하는 Git 명령어
명령어	설명	예시
git status	저장소의 상태를 확인하기 위해 사용하는 명령어
현재 브랜치의 이름과 추가변경된 파일 및 디렉토리 목록 표시	git status
git add	파일이나 디렉토리를 인덱스에 추가하는데 사용하는 명령어	git add [file_pattern]
git commit	인덱스에 추가된 파일이나 폴더의 내용을 저장소에 쓸때 사용하는 명령어
* git commit 옵션 "인덱스"	git commit -m "first commit"
git branch	브랜치에 대해 다양한 작업을 수행하기 위해 사용하는 명령어
* git branch -M [브랜치명] : 브랜치 만들기
* git branch : 브랜치 목록보기
* git branch -d [브랜치명] : 지정한 브랜치를 삭제	git branch -M main
git checkout	로컬 저장소의 브랜치를 전환할 때 사용하는 명령어
* git checkout [브랜치명] 	git checkout main 
git log	로컬 저장소의 커밋 히스토리를 탐색하는데 사용하는 명령
-n옵션으로 내역보기 수를 지정할 수 있습니다. 	git log -n 10
git grep	저장소의 파일 내용에서 검색하고나 할 때 사용하는 명령어
* git grep "검색 단어"	git grep "Hello"
git clone	기존 원격 저장소의 파일들을 로컬저장소에 다운로드하기 위하여 사용하는 명령어
* git clone [url]	git clone http://github.com/alvarotrigo/fullPage.js.git
git remote	원격 저장소를 조작하는데 사용하는 명령어
* git remote : 원격 저장소의 이름목록 표시
* git remote -v : 원격 저장소에 대한 자세한 목록 보기
* git remote add [원격저장소이름] [url] : 원격 저장소를 추가
* git remote rm [원격저장소이름] : 원격저장소 제거	 
git reset	로컬 저장소의 커밋을 취소하기 위해 사용하는 명령어
잘못 커밋하거나 수정이 누락되어 있을 때 자주 사용	git reset -soft HEAD ^
git merge	현재 브랜치에서 다른 지점에서 변경사항을 병합하는데 사용하는 명령어
다음 예시는 bugfix를 master 브랜치에 병합하는 내용	git checkout master git merge bugfix
git pull	원격 브랜치의 변경사항을 캡처하기 위해 사용하는 명령어
다음 예신느 로컬 저장소의 master브랜치에 원격 저장소 origin의 master브랜치를 가져옴	git checkout matser git pull origin master
 
 
 