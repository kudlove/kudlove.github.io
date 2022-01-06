---
title: '[MD] 마크다운 , 파이썬 공부시작'
excerpt: >-
  md 파일에 마크다운 문법으로 작성하여 Github 원격 저장소에 업로드 해보자. 에디터는 Visual Studio code 사용! 로컬
  서버에서 확인도 해보자. 
categories:
  - Blog
tags:
  - - Blog
    - jekyll
    - Github
    - Git
    - Python
toc: true
toc_sticky: true
date: {}
last_modified_at: {}
published: true
---

 ## 파이썬 사용 함수
***
- ### QT Style  
  https://doc.qt.io/qt-5/stylesheet-examples.html
- ### LINE Messaging API 사용해보기
  https://engineering.linecorp.com/ko/blog/line-messaging-api-samplebot/
- ### LINE Developers
  https://developers.line.biz/en/docs/messaging-api/
- ### Node.js와 Python으로 LINE Notify 사용해보기(1) – 기본
  https://engineering.linecorp.com/ko/blog/detail/334/

***
> 인증서 문제 해결 명령어  
  --trusted-host  
 ex )  pip --trusted-host pypi.org --trusted-host files.pythonhosted.org install jupyterlab 


> upgrade pip    
  python.exe -m pip  --trusted-host pypi.org --trusted-host files.pythonhosted.org install --upgrade pip  

> 주피터 사용하기 위해서  
  pip --trusted-host pypi.org --trusted-host files.pythonhosted.org install nbconvert
  
> C:\Users\kudlove\.jupyter\jupyter_lab_config.py



> 반올림  
  round() 


>버튼연결  
self.btnDel.clicked.connect(self.clickBtnDelete)

***    
    캘린더 위젯 이벤트 연결  
        self.calendarWidget.clicked.connect(self.calendarClicked)

*** 
    Key Event function
        def keyPressEvent(self, event):        
            super().keyPressEvent(event)
            keyEventProcess(self,event)  ## Event 처리 

***
    테이블 위젯 컬럼 정렬    
        self.tableWidget.item(cell.row(),0).setTextAlignment(Qt.AlignCenter | Qt.AlignVCenter)

    테이블 위젯 컬럼 가져오기  
        self.tableWidget.item(v, 2).text()

    테이블 위젯 컬럼 값 넣기  
         self.tableWidget.setItem( v, 6, QTableWidgetItem(str(winprice)))
    
    테이블 위젯 스타일 설정  
        #self.tableWidget.setStyleSheet("QHeaderView::section {background-color:#404040;color:#FFFFFF;}"); 
        self.tableWidget.setStyleSheet("QTableView::item:selected { color:white; background:#000000; font-weight:900; }"
                "QTableCornerButton::section { background-color:#232326; }"
                "QHeaderView::section { color:white; background-color:#232326; }")

***
    에디트 박스 정렬
        self.textEdit_1.setAlignment(Qt.AlignCenter) 

***   
    문자 순열 발생 ('123' -> '132' ....)

        from itertools import permutations

        perm = [''.join(p) for p in permutations(data)]
        set(perm) #중복삭제    
        new_list = []    
        for v in perm:    
            if v not in new_list:
                new_list.append(v)        

        for j in new_list:
            if data in new_list:
                new_list.remove(data)
