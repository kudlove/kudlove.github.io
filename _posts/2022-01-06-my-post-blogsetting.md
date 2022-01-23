---
title:  "[MD]블로그 세팅방법"
excerpt: "블로그 세팅정보를 기록하여 잊지안도록" 

categories:
  - Blog
tags:
  - [Blog, jekyll, Github, Git]

toc: true
toc_sticky: true


date: 2022-01-06
last_modified_at: 2021-01-10
---
# 루비,번들 설치

|Site|Address|
|---|:---:|
|루비|<https://www.ruby-lang.org/en/>|
|번들|<https://bundler.io/>|
|Github|[공부하는 식빵맘](https://ansohxxn.github.io/blog/posting/){: target="_blank"}|
|마크다운|[문법](https://hongsii.github.io/2017/06/01/How-to-Write-with-Markdown){: target="_blank"}|
|LINE 챗봇|[또삽질이구나](https://chooi9522.tistory.com/38){: target="_blank"}|

---
``` 
  로컬 서버에서 블로그에 적용될 모습 확인하기
  명령 프롬프트 cmd를 켜고 cd로 깃허브계정아이디. github.io 폴더로 이동한다.  
  bundle exec jekyll serve 명령
    -> 로컬 환경에서 jekyll 서버가 가동작성 중인 .md 파일을 저장하고  
  http://127.0.0.1:4000 로 접속    
    *예외*) Markdown Preview Enhanced 설치
```

    
# Javascript

```
  select 단일 객체
  $('select[name=SEND_TP]> option:selected').val()  
  $('select[name=SEND_TP]').attr("disabled", "disabled");

  select 배열 객체
  $("select[name='BF_IR_LEAK_FLAG']").eq(selectedIndex).val()

```

