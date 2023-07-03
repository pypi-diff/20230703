# Comparing `tmp/xython-1.3.0.tar.gz` & `tmp/xython-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xython-1.3.0.tar", last modified: Fri Jun 16 11:47:26 2023, max compression
+gzip compressed data, was "xython-1.4.0.tar", last modified: Mon Jul  3 11:47:17 2023, max compression
```

## Comparing `xython-1.3.0.tar` & `xython-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 11:47:25.999299 xython-1.3.0/
--rw-rw-rw-   0        0        0      388 2023-06-05 14:30:55.000000 xython-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9250 2023-06-16 11:47:26.000298 xython-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     8722 2023-06-05 14:30:55.000000 xython-1.3.0/README.md
--rw-rw-rw-   0        0        0        0 2021-06-11 06:00:16.000000 xython-1.3.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-06-16 11:47:26.002302 xython-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-16 11:44:48.000000 xython-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:47:25.926703 xython-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:47:25.976299 xython-1.3.0/src/xython/
--rw-rw-rw-   0        0        0      467 2023-06-16 11:39:36.000000 xython-1.3.0/src/xython/__init__.py
--rw-rw-rw-   0        0        0    23237 2023-06-11 00:05:23.000000 xython-1.3.0/src/xython/anydb.py
--rw-rw-rw-   0        0        0    86340 2023-06-13 13:09:23.000000 xython-1.3.0/src/xython/basic_data.py
--rw-rw-rw-   0        0        0    24552 2023-05-23 21:32:30.000000 xython-1.3.0/src/xython/ganada.py
--rw-rw-rw-   0        0        0    32173 2023-04-30 08:12:33.000000 xython-1.3.0/src/xython/gfinder.py
--rw-rw-rw-   0        0        0    19604 2023-05-22 13:41:17.000000 xython-1.3.0/src/xython/jfinder.py
--rw-rw-rw-   0        0        0    24532 2023-05-23 21:32:30.000000 xython-1.3.0/src/xython/mailmail.py
--rw-rw-rw-   0        0        0   144097 2023-06-16 10:51:24.000000 xython-1.3.0/src/xython/pcell.py
--rw-rw-rw-   0        0        0     5736 2023-04-08 04:25:55.000000 xython-1.3.0/src/xython/pcell_event.py
--rw-rw-rw-   0        0        0    11415 2023-05-22 13:34:23.000000 xython-1.3.0/src/xython/pyclick.py
--rw-rw-rw-   0        0        0    36331 2023-05-23 20:51:47.000000 xython-1.3.0/src/xython/pynal.py
--rw-rw-rw-   0        0        0    35958 2023-06-16 10:41:29.000000 xython-1.3.0/src/xython/scolor.py
--rw-rw-rw-   0        0        0    53568 2023-06-16 11:26:16.000000 xython-1.3.0/src/xython/youtil.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:47:25.997298 xython-1.3.0/src/xython.egg-info/
--rw-rw-rw-   0        0        0     9250 2023-06-16 11:47:25.000000 xython-1.3.0/src/xython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-16 11:47:25.000000 xython-1.3.0/src/xython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 11:47:25.000000 xython-1.3.0/src/xython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 14:32:10.000000 xython-1.3.0/src/xython.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-16 11:47:25.000000 xython-1.3.0/src/xython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 11:47:17.279041 xython-1.4.0/
+-rw-rw-rw-   0        0        0      388 2023-06-05 14:30:55.000000 xython-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10625 2023-07-03 11:47:17.279041 xython-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9035 2023-06-16 12:39:01.000000 xython-1.4.0/README.md
+-rw-rw-rw-   0        0        0        0 2021-06-11 06:00:16.000000 xython-1.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-03 11:47:17.285994 xython-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-07-03 11:26:20.000000 xython-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:47:17.107616 xython-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 11:47:17.248857 xython-1.4.0/src/xython/
+-rw-rw-rw-   0        0        0      467 2023-07-03 11:15:08.000000 xython-1.4.0/src/xython/__init__.py
+-rw-rw-rw-   0        0        0    23487 2023-06-28 11:43:49.000000 xython-1.4.0/src/xython/anydb.py
+-rw-rw-rw-   0        0        0    86378 2023-06-29 13:12:33.000000 xython-1.4.0/src/xython/basic_data.py
+-rw-rw-rw-   0        0        0    24689 2023-06-27 12:35:21.000000 xython-1.4.0/src/xython/ganada.py
+-rw-rw-rw-   0        0        0    19727 2023-06-27 10:43:06.000000 xython-1.4.0/src/xython/jfinder.py
+-rw-rw-rw-   0        0        0    25128 2023-06-28 11:34:56.000000 xython-1.4.0/src/xython/mailmail.py
+-rw-rw-rw-   0        0        0   165114 2023-07-01 11:36:47.000000 xython-1.4.0/src/xython/pcell.py
+-rw-rw-rw-   0        0        0     5736 2023-04-08 04:25:55.000000 xython-1.4.0/src/xython/pcell_event.py
+-rw-rw-rw-   0        0        0     9224 2023-06-27 12:05:29.000000 xython-1.4.0/src/xython/pyclick.py
+-rw-rw-rw-   0        0        0    59645 2023-06-28 11:29:46.000000 xython-1.4.0/src/xython/pynal.py
+-rw-rw-rw-   0        0        0    35896 2023-06-27 10:56:24.000000 xython-1.4.0/src/xython/scolor.py
+-rw-rw-rw-   0        0        0    78637 2023-06-29 10:37:55.000000 xython-1.4.0/src/xython/youtil.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:47:17.274025 xython-1.4.0/src/xython.egg-info/
+-rw-rw-rw-   0        0        0    10625 2023-07-03 11:47:16.000000 xython-1.4.0/src/xython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-07-03 11:47:17.000000 xython-1.4.0/src/xython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 11:47:16.000000 xython-1.4.0/src/xython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:47:16.000000 xython-1.4.0/src/xython.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-03 11:47:16.000000 xython-1.4.0/src/xython.egg-info/top_level.txt
```

### Comparing `xython-1.3.0/PKG-INFO` & `xython-1.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,140 @@
 Metadata-Version: 2.1
 Name: xython
-Version: 1.3.0
+Version: 1.4.0
 Summary: Easy Read / Write for Excel, Word, Color, Etc using Python
 Home-page: https://github.com/sjpark/xython
-Download-URL: https://github.com/sjpark/xython/archive/v1.3.0.tar.gz
 Author: sjpark
 Author-email: sjpkorea@yahoo.com
+License: UNKNOWN
+Download-URL: https://github.com/sjpark/xython/archive/v1.4.0.tar.gz
+Description: ## xython 모듈에 대하여
+        ### 개괄적인 설명
+        이모듈은 업무용으로 많이 사용하는 엑셀 , 색, 정규표현식, 등에 대하여 Python과 win32com을 기본으로 사용하여 각기 새롭게 모듈을 만들어서 좀더 쉽고 편하게 사용하고 만들자는 것입니다
+        자동화는 각자의 사용에 대한  
+        
+        만든 이유는 우리가 업무등을 하는 입장에서, 손으로 작업하기에는 양이 많고, 그렇다고
+        계속 반복적으로 일어나는 일은 아니며, VBA등을 만들어서 사용하기에는 어렵고 힘든 부분에 대해서
+        
+        파이썬이라는 훌룡한 언어를 위용하여, 좀더 쉽고 간결하게 몇가지 기능만 배워도 20줄안으로 자신만의 코드를
+        만들어 사용할수있는 기준을 만들기 위한 것입니다
+        
+        또한 보통 많이 사용하는 코드들은 첨부된 sample코드를 보시거나 저의 사이트에 와서 비슷한것을 다운 받은후
+        변경해서 사용하시기를 추천 드립니다
+        
+        좀더 편한 업무의 일을 하기위한 것입니다
+        
+        ### 구성은 
+        
+            - pcell : 엑셀을 다루는 것
+            - pcell_event : 엑셀의 이벤트를 다루는것
+            - scolor : 색의 RGB값을 편하게 사용가능하도록 만든 것
+            - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
+            - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
+            - ganada : 워드를 다루기위해 만든 것
+            - mailmail : outlook을 다루는것
+            - pyclick : 키보드와 마우스를 다루는 모듈
+            - pynal : 시간과 날짜를 다루는것
+            - youtil : 이러저런 문장이나 시간등을 변환하는데 도움이되는 것
+            - basic_data : halmoney패키지에서 사용되는 전반적인 공유 자료들을 저장하는 곳
+        
+        각 사용사용방법들에 대해서는 아래의 사이트를 참고하세요
+        
+        * https://cafe.naver.com/pycell
+        * www.halmoney.com
+        * www.xython.co.kr
+        
+        
+        ## 기본 사용법
+        ### pcell
+        -각 메소드는 각각 별도의 내용으로 사용합니다
+        
+        Pcell의 모듈을 만들 때 나름대로 편하고 쉽게 이름을 만들려고 하였습니다. 기본적인 틀을 만들어 놓으니, 분명억지로 지어진 이름또한 있음을 시인합니다. 나름대로 생각하고 고심한끝에 만들어진 이름이오니 맘에 들지 않는 부분이 있이더라도 양해를 부탁드립니다
+        
+        물론, 지금의 이름이 최종이라고는 생각하지 않고 있습니다. 좋은 이름이라는것은 어떤 메소드가 들어가 있는지 잘 몰라도 거의 사용하는데 사람의 생각에서 쉽게 사용을 할수 있도록 만드는 것이라고 생각을 합니다
+        
+        아마 한 4~5번정오는 크게 이름을 변경한 것 같습니다. 만들어놓고 조금지나면 저스스로가 도데체 이것의 이름은 왜 이렇게 만들어놓은거야???라는 질문을 하는경우가 가끔있습니다. 이리바꾸고 저리바꾸어도 맘에 안드는구석이 아직 많습니다
+        
+        한사람의 이름이 인생에서 차지하는부분이 많듯이 제가만든것또한 그러하지만, 만약 맘에 안드시는 것이 있으시면 본인스스로가 바꾼어서 사용하셔도 됩니다
+        
+        단, 기존의것은 그대로 두시고 아래부분에 새로운 메소드를 추가하셔서 위의것을 그대로 사용하시면 될것입니다
+        
+        그래서 다음과 같은 원리를 이용해서 만들었으나, 조금은 틀린부분도 있지만…
+        
+        	1. 이름은 기본적으로 3부분으로 만들었으며 각부분은 언더바(_)로 연결했습니다
+        	2. 읽을때는 read, 쓸때는 write, 삭제는 delete, 추가는insert등을 사용하였습니다
+        	3. 두번째의 이름의 규칙은
+        		관련된 부분에 따라 다른것을 사용하며 다음과 같은 것이 사용이 됩니다
+        		거진 영역을 나타내는 부분으로 사용하였습니다
+        		range, workbook, cell, line, column
+        	4. 세번째 부분이 어떤 일을 할것인지를 알아보는 것입니다
+        	5. 일반사항은 다음과 같습니다
+        
+        -	모든함수에는 sheet가 명시되어야 합니다
+        -	값을 읽는것은 read로 시작하며
+        -	값을 쓰는 것은 write로 시작합니다
+        -	선을 긋는등의 그림은 dwg로 시작합니다
+        -	하나의 자료가 아닌, 자료의 묶음은 Range를 사용한다
+        -	두개의 문구사이에는 '_' 로 연결을 하였다 예) read_cell
+        -	메소드는 모두 소문자를 사용함
+        
+        예를 들어, 어떤셀에 값을 입력하는 것은 write_value_in_cell라는 이름으로 구성하였습니다
+        그리고 부가적으로 함수의 변수로 사용되는부분은 큰 것->작은것으로 만들었으며, 영역을 표시하는 부분은 모두 리스트를 기준으로 하나로 만들었습니다.
+        
+        그저, 그렇다는것을 이해바라며, 실질적으로 코드를 보시면 더 쉽게 이해가 가실것으로 생각됩니다.
+        보지않고 찾지않아도 함수의 이름을 생각해낼수있도록 만든다고 나름대로 정의한 것입니다.
+        
+        ### scolor
+        이것은 모든 외부로 들어오고 나가는 것은 전부 RGB형태로 이루어지도록 만든다
+        
+            - 색을 변경하고 관리하는 모듈이며
+            - 색의 변화를 잘 사용이 가능하도록 하기위한 것이다
+            - 기본 입력 예 : "빨강", "빨강55", "red55", "0155"
+            - 기본색 ==> 12색 + (하양, 검정, 회색),
+            - 큰변화 ==> 1~9단계, 작은변화 ==> 1~9단계
+            - 기본함수 : get_color_rgb("red55"), get_rgb_3input(색, 큰변화, 작은변화)
+            - 모든 색의 표현이나 결과는 rgb로 돌려준다
+        
+        ### Jfinder
+        이름을 **Jfinder**라고 지었으며, 아래와 같은 특성을 가지고 있다
+        
+        1. 건수는 ~를 사용하여 4~5라는 식으로 표현을 하였고
+        2. 한글, 영어와 같은 것은 대괄호를 사용하여 적용하였다 [한글]
+        3. 처음과 끝은 [처음], [끝]처럼 나타냈다
+        4. 그리고 이것은 누가 보아도 아~~ 무엇을 찾을려고 했는지를 알수있도록 하기위한것이며
+        5. 찾기기능중에 전부 찾아서 보기쉽도록 돌려주는 것과 같은 몇가지 메소드들을 만들어 넣었읍니다
+        제일 중요한 코드를 만드는 기능은 아래와 같읍니다
+        대략적으로 위의것을 읽은후에 보시면 이해가 되실부분이 많읍니다
+        
+        * 아래의 코드들은 정규표현식을 사용하면서, 내가 만든 표현식조차도 다시 읽기가 어려워서, 나름 다른 형태로 만들어 본것인데. 생각보다 가독성이 좋아서 같이 공유해보는것이다
+        또한 만든김에 결과로 돌려주는것도 하나만 받으면 전부 가능하도록 만들어 보았다
+        위에서 언급한 이메일 형식이 맞느지를 보는 것은 상당히 반복적이기 때문에 크게 혼돈은 없다
+        하지만, 실제 코드를 사용하다 보면, 외계어를 해석하는 상태까지 와야할 경우가 있다
+        
+        
+            ([a-zA-Z0-9_.+-]+)@[a-zA-Z0-9_.+-]+\.[a-zA-Z0-9_.+-]+
+        
+        * 이정도만해도 간단한 축에 속한다. 맨처음 만들때는 그나마 이해를 하지만, 다른사람이 만든 것을 이해하는데 상당한 시간이 걸린다는 것이고, 또한 일반적인 사용자들이 이것을 공부하고 이해하는데 어려움이 잇을 것 같으면서 동시에, 정규표현식의 강력함을 사용할수 있도록 생각해 보는 것이다
+        그래서 좀더 간단하게 사용법을 만들고,
+        
+        
+            [영어&숫자.+-:1~]@[영어&숫자.+-:1~]\.[영어&숫자.+-:1~]
+        이렇게 바꾸면 좀더 읽기가 쉬워진다
+        
+        **jfinder**에는 자주사용하는 언어를 등록할수도 있읍니다. 예를 들어 일본어나 한자를 등록한것처럼 하면 사용이 가능하다.
+        간단하게 다시 사용하는 방법을 알려주면, 너무 줄여놓은 정규표현식을 좀더 늘이는 것이라고 생각하면 됩니다. 여기에서 느낀 부분은 전문가가 사용하기에는 좋지만, 비전문가가 사용하기 쉽게, 예전에는 단어1개가 아주 중요한 속도까지 영향을 주지만, 지금은너무 줄이지 않아도 된다는 것이다. 기계에 가까운 언어에서 좀더 사용자에 가까운 언어로 만들어도 된다는 것이지요
+        파이선이 사용하기에 좀더 편한방법이 되는 것이지요
+        
+            - 대괄호로 묶는다
+            - 반복갯수는 대괄호안에 사용하며 ~로 나타낸다
+            - 맨처음 맨마지막등의 용어는 [처음], [끝]등의 이유로 나타낸다 
+            - 특수문자(re모듈내에 의미가있는 문자)는 \를 붙여서 사용한다
+            - 어떤문자의 앞과뒤에있을때는 (앞에있음:abc)이라고 사용하면 abc가 앞에있는 문자열을 찾는것이다
+        
+        ### mailmail
+        이름을 **mailmail**라고 지었으며, 아웃룩의 이메일을 관리하는 도구입니다
+        - 이것의 장점은 엑셀이나 Util과 연동하여 편의성을 더욱 증대하고있읍니다
+        - 기본적인 사용법이나 함수의 이름은 같은 형태를 따릅니다
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-
-## xython 모듈에 대하여
-### 개괄적인 설명
-이모듈은 업무용으로 많이 사용하는 엑셀 , 색, 정규표현식, 등에 대하여 Python과 win32com을 기본으로 사용하여 각기 새롭게 모듈을 만들어서 좀더 쉽고 편하게 사용하고 만들자는 것입니다
-자동화는 각자의 사용에 대한  
-
-만든 이유는 우리가 업무등을 하는 입장에서, 손으로 작업하기에는 양이 많고, 그렇다고
-계속 반복적으로 일어나는 일은 아니며, VBA등을 만들어서 사용하기에는 어렵고 힘든 부분에 대해서
-
-파이썬이라는 훌룡한 언어를 위용하여, 좀더 쉽고 간결하게 몇가지 기능만 배워도 20줄안으로 자신만의 코드를
-만들어 사용할수있는 기준을 만들기 위한 것입니다
-
-또한 보통 많이 사용하는 코드들은 첨부된 sample코드를 보시거나 저의 사이트에 와서 비슷한것을 다운 받은후
-변경해서 사용하시기를 추천 드립니다
-
-좀더 편한 업무의 일을 하기위한 것입니다
-
-### 구성은 
-
-    - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
-    - basic_data : halmoney패키지에서 사용되는 전반적인 공유 자료들을 저장하는 곳
-    - ganada : 워드를 다루기위해 만든 것
-    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
-    - mailmail : outlook을 다루는것
-    - pcell : 엑셀을 다루는 것
-    - pcell_event : 엑셀의 이벤트를 다루는것
-    - pyclick : 키보드와 마우스를 다루는 모듈
-    - pynal : 시간과 날짜를 다루는것
-    - scolor : 색의 RGB값을 편하게 사용가능하도록 만든 것
-    - youtil : 이러저런 문장이나 시간등을 변환하는데 도움이되는 것
-
-각 사용사용방법들에 대해서는 아래의 사이트를 참고하세요
-
-* https://cafe.naver.com/pycell
-* www.halmoney.com
-
-
-## 기본 사용법
-### pcell
--각 메소드는 각각 별도의 내용으로 사용합니다
-
-Pcell의 모듈을 만들 때 나름대로 편하고 쉽게 이름을 만들려고 하였습니다. 기본적인 틀을 만들어 놓으니, 분명억지로 지어진 이름또한 있음을 시인합니다. 나름대로 생각하고 고심한끝에 만들어진 이름이오니 맘에 들지 않는 부분이 있이더라도 양해를 부탁드립니다
-
-물론, 지금의 이름이 최종이라고는 생각하지 않고 있습니다. 좋은 이름이라는것은 어떤 메소드가 들어가 있는지 잘 몰라도 거의 사용하는데 사람의 생각에서 쉽게 사용을 할수 있도록 만드는 것이라고 생각을 합니다
-
-아마 한 4~5번정오는 크게 이름을 변경한 것 같습니다. 만들어놓고 조금지나면 저스스로가 도데체 이것의 이름은 왜 이렇게 만들어놓은거야???라는 질문을 하는경우가 가끔있습니다. 이리바꾸고 저리바꾸어도 맘에 안드는구석이 아직 많습니다
-
-한사람의 이름이 인생에서 차지하는부분이 많듯이 제가만든것또한 그러하지만, 만약 맘에 안드시는 것이 있으시면 본인스스로가 바꾼어서 사용하셔도 됩니다
-
-단, 기존의것은 그대로 두시고 아래부분에 새로운 메소드를 추가하셔서 위의것을 그대로 사용하시면 될것입니다
-
-그래서 다음과 같은 원리를 이용해서 만들었으나, 조금은 틀린부분도 있지만…
-
-	1. 이름은 기본적으로 3부분으로 만들었으며 각부분은 언더바(_)로 연결했습니다
-	2. 읽을때는 read, 쓸때는 write, 삭제는 delete, 추가는insert등을 사용하였습니다
-	3. 두번째의 이름의 규칙은
-		관련된 부분에 따라 다른것을 사용하며 다음과 같은 것이 사용이 됩니다
-		거진 영역을 나타내는 부분으로 사용하였습니다
-		range, workbook, cell, line, column
-	4. 세번째 부분이 어떤 일을 할것인지를 알아보는 것입니다
-	5. 일반사항은 다음과 같습니다
-
--	모든함수에는 sheet가 명시되어야 합니다
--	값을 읽는것은 read로 시작하며
--	값을 쓰는 것은 write로 시작합니다
--	선을 긋는등의 그림은 dwg로 시작합니다
--	하나의 자료가 아닌, 자료의 묶음은 Range를 사용한다
--	두개의 문구사이에는 '_' 로 연결을 하였다 예) read_cell
--	메소드는 모두 소문자를 사용함
-
-예를 들어, 어떤셀에 값을 입력하는 것은 write_value_in_cell라는 이름으로 구성하였습니다
-그리고 부가적으로 함수의 변수로 사용되는부분은 큰 것->작은것으로 만들었으며, 영역을 표시하는 부분은 모두 리스트를 기준으로 하나로 만들었습니다.
-
-그저, 그렇다는것을 이해바라며, 실질적으로 코드를 보시면 더 쉽게 이해가 가실것으로 생각됩니다.
-보지않고 찾지않아도 함수의 이름을 생각해낼수있도록 만든다고 나름대로 정의한 것입니다.
-
-### scolor
-이것은 모든 외부로 들어오고 나가는 것은 전부 RGB형태로 이루어지도록 만든다
-
-    - 색을 변경하고 관리하는 모듈이며
-    - 색의 변화를 잘 사용이 가능하도록 하기위한 것이다
-    - 기본 입력 예 : "빨강", "빨강55", "red55", "0155"
-    - 기본색 ==> 12색 + (하양, 검정, 회색),
-    - 큰변화 ==> 1~9단계, 작은변화 ==> 1~9단계
-    - 기본함수 : get_color_rgb("red55"), get_rgb_3input(색, 큰변화, 작은변화)
-    - 모든 색의 표현이나 결과는 rgb로 돌려준다
-
-### Jfinder
-이름을 **Jfinder**라고 지었으며, 아래와 같은 특성을 가지고 있다
-
-1. 건수는 ~를 사용하여 4~5라는 식으로 표현을 하였고
-2. 한글, 영어와 같은 것은 대괄호를 사용하여 적용하였다 [한글]
-3. 처음과 끝은 [처음], [끝]처럼 나타냈다
-4. 그리고 이것은 누가 보아도 아~~ 무엇을 찾을려고 했는지를 알수있도록 하기위한것이며
-5. 찾기기능중에 전부 찾아서 보기쉽도록 돌려주는 것과 같은 몇가지 메소드들을 만들어 넣었읍니다
-제일 중요한 코드를 만드는 기능은 아래와 같읍니다
-대략적으로 위의것을 읽은후에 보시면 이해가 되실부분이 많읍니다
-
-* 아래의 코드들은 정규표현식을 사용하면서, 내가 만든 표현식조차도 다시 읽기가 어려워서, 나름 다른 형태로 만들어 본것인데. 생각보다 가독성이 좋아서 같이 공유해보는것이다
-또한 만든김에 결과로 돌려주는것도 하나만 받으면 전부 가능하도록 만들어 보았다
-위에서 언급한 이메일 형식이 맞느지를 보는 것은 상당히 반복적이기 때문에 크게 혼돈은 없다
-하지만, 실제 코드를 사용하다 보면, 외계어를 해석하는 상태까지 와야할 경우가 있다
-
-
-    ([a-zA-Z0-9_.+-]+)@[a-zA-Z0-9_.+-]+\.[a-zA-Z0-9_.+-]+
-
-* 이정도만해도 간단한 축에 속한다. 맨처음 만들때는 그나마 이해를 하지만, 다른사람이 만든 것을 이해하는데 상당한 시간이 걸린다는 것이고, 또한 일반적인 사용자들이 이것을 공부하고 이해하는데 어려움이 잇을 것 같으면서 동시에, 정규표현식의 강력함을 사용할수 있도록 생각해 보는 것이다
-그래서 좀더 간단하게 사용법을 만들고,
-
-
-    [영어&숫자.+-:1~]@[영어&숫자.+-:1~]\.[영어&숫자.+-:1~]
-이렇게 바꾸면 좀더 읽기가 쉬워진다
-
-**jfinder**에는 자주사용하는 언어를 등록할수도 있읍니다. 예를 들어 일본어나 한자를 등록한것처럼 하면 사용이 가능하다.
-간단하게 다시 사용하는 방법을 알려주면, 너무 줄여놓은 정규표현식을 좀더 늘이는 것이라고 생각하면 됩니다. 여기에서 느낀 부분은 전문가가 사용하기에는 좋지만, 비전문가가 사용하기 쉽게, 예전에는 단어1개가 아주 중요한 속도까지 영향을 주지만, 지금은너무 줄이지 않아도 된다는 것이다. 기계에 가까운 언어에서 좀더 사용자에 가까운 언어로 만들어도 된다는 것이지요
-파이선이 사용하기에 좀더 편한방법이 되는 것이지요
-
-    - 대괄호로 묶는다
-    - 반복갯수는 대괄호안에 사용하며 ~로 나타낸다
-    - 맨처음 맨마지막등의 용어는 [처음], [끝]등의 이유로 나타낸다 
-    - 특수문자(re모듈내에 의미가있는 문자)는 \를 붙여서 사용한다
-    - 어떤문자의 앞과뒤에있을때는 (앞에있음:abc)이라고 사용하면 abc가 앞에있는 문자열을 찾는것이다
```

### Comparing `xython-1.3.0/README.md` & `xython-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 또한 보통 많이 사용하는 코드들은 첨부된 sample코드를 보시거나 저의 사이트에 와서 비슷한것을 다운 받은후
 변경해서 사용하시기를 추천 드립니다
 
 좀더 편한 업무의 일을 하기위한 것입니다
 
 ### 구성은 
 
+    - pcell : 엑셀을 다루는 것
+    - pcell_event : 엑셀의 이벤트를 다루는것
+    - scolor : 색의 RGB값을 편하게 사용가능하도록 만든 것
+    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
     - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
-    - basic_data : halmoney패키지에서 사용되는 전반적인 공유 자료들을 저장하는 곳
     - ganada : 워드를 다루기위해 만든 것
-    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
     - mailmail : outlook을 다루는것
-    - pcell : 엑셀을 다루는 것
-    - pcell_event : 엑셀의 이벤트를 다루는것
     - pyclick : 키보드와 마우스를 다루는 모듈
     - pynal : 시간과 날짜를 다루는것
-    - scolor : 색의 RGB값을 편하게 사용가능하도록 만든 것
     - youtil : 이러저런 문장이나 시간등을 변환하는데 도움이되는 것
+    - basic_data : halmoney패키지에서 사용되는 전반적인 공유 자료들을 저장하는 곳
 
 각 사용사용방법들에 대해서는 아래의 사이트를 참고하세요
 
 * https://cafe.naver.com/pycell
 * www.halmoney.com
+* www.xython.co.kr
 
 
 ## 기본 사용법
 ### pcell
 -각 메소드는 각각 별도의 내용으로 사용합니다
 
 Pcell의 모듈을 만들 때 나름대로 편하고 쉽게 이름을 만들려고 하였습니다. 기본적인 틀을 만들어 놓으니, 분명억지로 지어진 이름또한 있음을 시인합니다. 나름대로 생각하고 고심한끝에 만들어진 이름이오니 맘에 들지 않는 부분이 있이더라도 양해를 부탁드립니다
@@ -114,8 +115,13 @@
 간단하게 다시 사용하는 방법을 알려주면, 너무 줄여놓은 정규표현식을 좀더 늘이는 것이라고 생각하면 됩니다. 여기에서 느낀 부분은 전문가가 사용하기에는 좋지만, 비전문가가 사용하기 쉽게, 예전에는 단어1개가 아주 중요한 속도까지 영향을 주지만, 지금은너무 줄이지 않아도 된다는 것이다. 기계에 가까운 언어에서 좀더 사용자에 가까운 언어로 만들어도 된다는 것이지요
 파이선이 사용하기에 좀더 편한방법이 되는 것이지요
 
     - 대괄호로 묶는다
     - 반복갯수는 대괄호안에 사용하며 ~로 나타낸다
     - 맨처음 맨마지막등의 용어는 [처음], [끝]등의 이유로 나타낸다 
     - 특수문자(re모듈내에 의미가있는 문자)는 \를 붙여서 사용한다
-    - 어떤문자의 앞과뒤에있을때는 (앞에있음:abc)이라고 사용하면 abc가 앞에있는 문자열을 찾는것이다
+    - 어떤문자의 앞과뒤에있을때는 (앞에있음:abc)이라고 사용하면 abc가 앞에있는 문자열을 찾는것이다
+
+### mailmail
+이름을 **mailmail**라고 지었으며, 아웃룩의 이메일을 관리하는 도구입니다
+- 이것의 장점은 엑셀이나 Util과 연동하여 편의성을 더욱 증대하고있읍니다
+- 기본적인 사용법이나 함수의 이름은 같은 형태를 따릅니다
```

### Comparing `xython-1.3.0/setup.py` & `xython-1.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
-#with open("README.md", "rt", encoding='UTF8') as fh:
-#    long_description = fh.read()
+with open("README.md", "rt", encoding='UTF8') as fh:
+    long_description = fh.read()
 setup(
     name='xython',
-    version='1.3.0',
+    version='1.4.0',
     url='https://github.com/sjpark/xython',
-    download_url='https://github.com/sjpark/xython/archive/v1.3.0.tar.gz',
+    download_url='https://github.com/sjpark/xython/archive/v1.4.0.tar.gz',
     author='sjpark',
     author_email='sjpkorea@yahoo.com',
     description='Easy Read / Write for Excel, Word, Color, Etc using Python',
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,
     package_data={
         "xython": ["*.*"],
         },
     long_description_content_type="text/markdown",
     long_description=open('README.md', "r", encoding='UTF8').read(),
     install_requires=[''],
-    python_requires='>=3.9',
+    python_requires='>=3.8',
     zip_safe=False,
     classifiers=['License :: OSI Approved :: MIT License'],
     )
```

### Comparing `xython-1.3.0/src/xython/anydb.py` & `xython-1.4.0/src/xython/anydb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 import os  # 내장모듈
 import sqlite3  # 내장모듈
 import pickle #내장모듈
 
-import youtil  # halmoney 모듈
-import pcell  # halmoney 모듈
+import youtil  # xython 모듈
+import pcell  # xython 모듈
+import basic_data  # xython 모듈
 
 import pandas as pd
 import numpy as np
 
 class anydb:
 	"""
 	database를 사용하기 쉽게 만든것
@@ -17,16 +18,24 @@
 
 	def __init__(self, db_name=""):
 		self.yt = youtil.youtil()
 		self.db_name = db_name
 		self.table_name = ""
 
 		self.con = ""  # sqlite db에 연결되는 것
-		self.cursor = ""
+		if db_name =="":
+			pass
+		else:
+			self.con = sqlite3.connect(db_name, isolation_level=None)
+			self.cursor = self.con.cursor()
 		self.make_connection_with_sqlite_db(self.db_name)
+		self.base_data = basic_data.basic_data()
+		self.var = self.base_data.vars
+		self.var_common={}
+
 
 	def append_df1_df2(self, df_obj_1, df_obj_2):
 		"""
 		dataframe끝에 dataframe형태의 자료를 추가하는것
 		"""
 		result = pd.concat([df_obj_1, df_obj_2])
 		return result
```

### Comparing `xython-1.3.0/src/xython/basic_data.py` & `xython-1.4.0/src/xython/basic_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,17 +63,164 @@
 		함수이름 : 액션_행위설명_범위_설명, Write_value_in_cell_by_limit
 		"""
 		return result
 
 	def __init__(self):
 		self.vars = {}
 
-		self.vars["basic_color_step"] = ["+++++", "++++", "+++", "++", "+", "", "-", "--", "---", "----", "-----"]
+		self.vars["list_알파벳"] = "abcdefghijklmnopqrstuvwxyz"
+		self.vars["list_자음"] = "ㄱㄴㄷㄹㅁㅂㅅㅇㅈㅊㅋㅌㅍㅎ"
+		self.vars["list_모음"] ="ㅏㅑㅓㅕㅗㅛㅜㅠㅡㅣ"
+		self.vars["list_자음_19"] = self.vars["first_letter"] = ["ㄱ", "ㄲ", "ㄴ", "ㄷ", "ㄸ", "ㄹ", "ㅁ", "ㅂ", "ㅃ", "ㅅ", "ㅆ", "ㅇ", "ㅈ", "ㅉ", "ㅊ", "ㅋ", "ㅌ", "ㅍ", "ㅎ"]  # 19 글자
+		self.vars["list_모음_21"] = self.vars["second_letter"] = ["ㅏ", "ㅐ", "ㅑ", "ㅒ", "ㅓ", "ㅔ", "ㅕ", "ㅖ", "ㅗ", "ㅘ", "ㅙ", "ㅚ", "ㅛ", "ㅜ", "ㅝ", "ㅞ", "ㅟ", "ㅠ", "ㅡ", "ㅢ", "ㅣ"]  # 21 글자
+		self.vars["list_받침_28"] = self.vars["third_letter"] = ["", "ㄱ", "ㄲ", "ㄳ", "ㄴ", "ㄵ", "ㄶ", "ㄷ", "ㄹ", "ㄺ", "ㄻ", "ㄼ", "ㄽ", "ㄾ", "ㄿ", "ㅀ", "ㅁ", "ㅂ", "ㅄ", "ㅅ", "ㅆ", "ㅇ", "ㅈ", "ㅊ", "ㅋ", "ㅌ", "ㅍ", "ㅎ"]  # 28 글자, 없는것 포함
+		self.vars["list_가나다"] = "가나다라마바사아자차카타파하"
+		self.vars["list_숫자"]= "1234567890"
+		self.vars["list_그리스문자"]= "αβγδεζήθικλμνξόπρΣτ"
+		self.vars["list_로마숫자"] = "ⅠⅡⅢⅣⅤⅥⅦⅧⅨⅩ"
+		self.vars["list_원ㄱ"] = "㉠㉡㉢㉣㉤㉥㉦㉧㉨㉩㉪㉫㉬㉭"
+		self.vars["list_원가"] = "㉮㉯㉰㉱㉲㉳㉴㉵㉶㉷㉸㉹㉺㉻"
+		self.vars["list_원a"] = "ⒶⒷⒸⒹⒺⒻⒼⒽⒾⒿⓀⓁⓂⓃⓄⓅⓆⓇⓈⓉⓊⓋⓌⓍⓎⓏ"
+		self.vars["list_원1"] ="⓪①②③④⑤⑥⑦⑧⑨⑩⑪⑫⑬⑭⑮⑯⑰⑱⑲⑳㉑㉒㉓㉔㉕㉖㉗㉘㉙㉚㉛㉜㉝㉞㉟㊱㊲㊳㊴㊵㊶㊷㊸㊹㊺㊻㊼㊽㊾㊿"
+		self.vars["list_색강도"] = self.vars["basic_color_step"] = ["+++++", "++++", "+++", "++", "+", "", "-", "--", "---", "----", "-----"]
+
+
+
+		self.vars["list_달력_서수_영어"] = self.vars["list_서수"] = ['1ST', '2ND', '3RD', '4TH', '5TH', '6TH', '7TH', '8TH', '9TH', '10TH', '11TH', '12TH', '13TH', '14TH', '15TH', '16TH', '17TH', '18TH', '19TH', '20TH', '21ST', '22ND', '23RD', '24TH', '25TH', '26TH', '27TH', '28TH', '29TH', '30TH', '31ST']
+		self.vars["list_10까지_영어"] = self.vars["list_getdigit"] = ['one', 'two', 'three', 'four', 'five', 'six', 'seven', 'eight', 'nine']
+		self.vars["list_10단위_영어"] = self.vars["list_num_eng_00digit"] = ['twenty', 'thirty', 'forty', 'fifty', 'sixty', 'seventy', 'eighty', 'ninety']
+		self.vars["list_10_19_영어"] = self.vars["list_num_eng_10"] = ['ten', 'eleven', 'twelve', 'thirteen', 'fourteen', 'fifteen', 'sixteen', 'eighteen', 'nineteen']
+		self.vars["list_1000_단위_영어"] = self.vars["list_num_eng_unit_1000"] = ['thousand', 'million', 'billion', 'trillion']
+		self.vars["list_월이름_영어_short"] = self.vars["list_month_eng_short"] = ['JAN', 'FEB', 'MAR', 'APR', 'MAY', 'JUN', 'JUL', 'AUG', 'SEP', 'OCT', 'NOV', 'DEC']
+		self.vars["list_월이름_영어"] = self.vars["list_month_eng"] = ['JANUARY', 'FEBRUARY', 'MARCH', 'APRIL', 'MAY', 'JUNE', 'JULY', 'AUGUST', 'SEPTEMBER', 'OCTOBER', 'NOVEMBER', 'DECEMBER']
+
+
+
+
+		self.vars["list_색이름_기본12가지_영어"] = self.vars["color_name_for_basic_12_eng"] = ['red', 'ora', 'yel', 'gre_yel', 'gre', 'gre_cya', 'cya', 'blu_cya', 'blu', 'blu_mag', 'pin', 'red_mag']
+		self.vars["list_색이름_영어"] = self.vars["list_colorname_eng"] = ["red", "ora", "yel", "gre_yel", "gre", "gre_cya", "cya", "blu_cya", "blu", "blu_mag", "mag", "red_mag", "gra", "whi", "bla"]
+		self.vars["list_색이름_영어_short"] = self.vars["list_colorname_eng_short"] = ["r", "o", "y", "gre_yel", "g", "gre_cya", "c", "blu_cya", "b", "blu_mag", "m", "red_mag", "g", "w", "bl"]
+		self.vars["list_색이름_기본12가지_한글"] = self.vars["color_name_for_basic_12_kor"] = ['빨강', '오렌지', '노랑', '연두', '초록', '연초록', '하늘', '군청색', '파랑', '남색', '핑크', '자주']
+		self.vars["list_색이름_한글"] = self.vars["list_colorname_kor"] = ["빨강", "주황", "노랑", "연두", "초록", "연초록", "옥색", "청록", "파랑", "남색", "보라", "자홍", "회색", "흰색", "검정"]
+
+		self.vars["list_색스타일_영어"] = self.vars["list_colorstyle_eng"] = ["white", "pale", "light", "soft", "vivid", "dull", "deep", "dark", "black", "gray"]
+		self.vars["list_색스타일_영어_1"] = self.vars["list_colorstyle_eng"] = ["vivid", "bright", "strong", "deep", "light", "soft", "dull", "dark", "pale", "lightgrayish", "grayish", "darkgrayish"]
+		self.vars["list_색톤_영어"] = self.vars["color_tone_eng"] =["pale", "light_grayish", "grayish", "dark_grayish", "light", "soft", "dull", "dark", "bright", "strong", "deep", "vivid"]
+		self.vars["list_색톤"] = self.vars["list_colorstyle_kor"] = ["파스텔", "연한", "밝은", "흐린", "선명한", "기본", "탁한", "진한", "어두운", "회색", "검은", "검정"]
+		self.vars["list_색톤_1"] = self.vars["color_tone_kor"] = ["연한", "밝은회색", "회색", "어두운회색", "옅은", "부드러운", "탁한", "어두운", "밝은", "강한", "짙은", "선명한"]
+
+		self.vars["list_pccs_색이름"] = self.vars["list_colorname_pccs"] = ["v", "b", "s", "dp", "lt", "sf", "d", "dk", "p", "ltg", "g", "dkg"]
+		#self.vars["list_color_name_for_all_kor"] = list(set(self.vars["check_color_name_kor"].values()))
+		self.vars["list_currency_eng_last"] = ['no', 'one', 'dollars']
+		self.vars["list_num_last_cent"] = ['only', 'and one cent', 'and', 'cents']
+		#self.vars["check_color_name"] = self.vars["check_color_name_eng"]
+
+
+
+
+
+		self.vars["list_기본12색_rgb"] = self.vars["list_basic_12rgb"] = [[255, 0, 0], [255, 128, 0], [255, 255, 0], [128, 255, 0],	[0, 255, 0], [0, 255, 128], [0, 255, 255], [0, 128, 255], [0, 0, 255], [128, 0, 255], [255, 0, 255], [255, 0, 128], ]
+		self.vars["list_기본12색_hsl"] = self.vars["list_basic_12hsl"] = [[0, 100, 50], [30, 100, 50], [60, 100, 50], [90, 100, 50], [120, 100, 50],	 [150, 100, 50], [180, 100, 50], [210, 100, 50], [240, 100, 50], [270, 100, 50], [300, 100, 50], [330, 100, 50]]
+		self.vars["list_12단계_h값"] = self.vars["list_basic_12h"] = [0, 30, 60, 90, 120, 150, 180, 210, 240, 270, 300, 330]
+		self.vars["list_10단계_sl값"] = self.vars["list_basic_10sl"] = [[100, 0], [90, 10], [80, 20], [70, 30], [60, 40], [50, 50], [40, 60], [30, 70], [10, 80], [10, 90], [0, 100]]
+		self.vars["list_11단계_sl값"] = self.vars["list_basic_11sl"] = [[100, 0], [100, 10], [100, 20], [100, 30], [100, 40], [100, 50], [100, 60], [100, 70], [100, 80], [100, 90], [100, 100]]
+		self.vars["list_12단계_칼라스타일"] = self.vars["list_basic_12colorstyle"] = [[90, 50], [80, 30], [80, 50], [80, 70], [50, 20], [50, 40], [50, 60], [50, 80], [20, 20], [20, 40], [20, 60], [20, 80]]
+		self.vars["list_faber_스타일_sl값"] = self.vars["sl_no_for_faber_style"] = [[[100, 0], [100, 50], [0, 0]], [[0, 0], [0, 75], [0, 100]],[[100, 0], [25, 75], [0, 100]], [[25, 0], [10, 50], [0, 75]], [[100, 0], [0, 0], [0, 100]], [[25, 0], [10, 50], [0, 75], [25, 75]], ]
+		self.vars["list_12가지톤_sl값"] = self.vars["sl_no_for_12_color_tone"] = [[90, 50], [80, 30], [80, 50], [80, 70], [50, 20], [50, 40], [50, 60], [50, 80], [20, 20], [20, 40], [20, 60], [20, 80]]
+		self.vars["list_12단계_색스타일_sl값"] = self.vars["list_colorstyle_slno"] = [[90, 50], [80, 30], [80, 50], [80, 70], [50, 20], [50, 40], [50, 60], [50, 80], [20, 20], [20, 40], [20, 60], [20, 80]]
+		self.vars["list_10단계_sl값"] = self.vars["sl_no_for_basic_10"] = [[100, 0], [90, 10], [80, 20], [70, 30], [60, 40], [50, 50], [40, 60], [30, 70], [10, 80], [10, 90], [0, 100]]
+		self.vars["list_12단계_hsl값"] = self.vars["hsl_no_for_basic_12"] = [[0, 100, 50], [30, 100, 50], [60, 100, 50], [90, 100, 50], [120, 100, 50], [150, 100, 50], [180, 100, 50], [210, 100, 50], [240, 100, 50], [270, 100, 50], [300, 100, 50], [330, 100, 50]]
+		self.vars["list_11단계_sl값"] = self.vars["sl_no_for_basic_11"] = [[100, 0], [100, 10], [100, 20], [100, 30], [100, 40], [100, 50], [100, 60], [100, 70], [100, 80], [100, 90], [100, 100]]
+		self.vars["list_12단계_rgb값"] = self.vars["rgb_46_for_excel"] = [[255, 0, 0], [255, 128, 0], [255, 255, 0], [128, 255, 0],	[0, 255, 0], [0, 255, 128], [0, 255, 255], [0, 128, 255],	[0, 0, 255], [128, 0, 255], [255, 0, 255], [255, 0, 128], ]
+		self.vars["list_12단계_h값"] =self.vars["h_no_for_basic_12"] =[0, 30, 60, 90, 120, 150, 180, 210, 240, 270, 300, 330]
+
+
+
+
+
+		self.vars["dic_자음_vs_번호"] = self.vars["first_letter_no"] = {"ㄱ":0, "ㄲ":1, "ㄴ":2, "ㄷ":3, "ㄸ":4, "ㄹ":5, "ㅁ":6, "ㅂ":7, "ㅃ":8, "ㅅ":9, "ㅆ":10, "ㅇ":11, "ㅈ":12, "ㅉ":13, "ㅊ":14, "ㅋ":15, "ㅌ":16, "ㅍ":17, "ㅎ":18}  # 19 글자
+		self.vars["dic_모음_vs_번호"] = self.vars["second_letter_no"] = {"ㅏ":0, "ㅐ":1, "ㅑ":2, "ㅒ":3, "ㅓ":4, "ㅔ":5, "ㅕ":6, "ㅖ":7, "ㅗ":8, "ㅘ":9, "ㅙ":10, "ㅚ":11, "ㅛ":12, "ㅜ":13, "ㅝ":14, "ㅞ":15, "ㅟ":16, "ㅠ":17, "ㅡ":18, "ㅢ":19, "ㅣ":20}  # 21 글자
+		self.vars["dic_받침_vs_번호"] = self.vars["third_letter_no"] = {"":0, "ㄱ":1, "ㄲ":2, "ㄳ":3, "ㄴ":4, "ㄵ":5, "ㄶ":6, "ㄷ":7, "ㄹ":8, "ㄺ":9, "ㄻ":10, "ㄼ":11, "ㄽ":12, "ㄾ":13, "ㄿ":14, "ㅀ":15,"ㅁ":16, "ㅂ":17, "ㅄ":18, "ㅅ":19, "ㅆ":20, "ㅇ":21, "ㅈ":22, "ㅊ":23, "ㅋ":24, "ㅌ":25, "ㅍ":26, "ㅎ":27}  # 28 글자, 없는것 포함
+		self.vars["dic_색톤_12가지_vs_번호"] = self.vars["color_tone_12_kor_vs_index"] = {"연한": 0, "밝은회색": 1, "회색": 2, "어두운회색": 3, "옅은": 4, "부드러운": 5, "탁한": 6, "어두운": 7, "밝은": 8, "강한": 9, "짙은": 10, "선명한": 11}
+		self.vars["dic_색톤_영어_vs_sl값"] = self.vars["color_tone_simple_eng_vs_sl_no"] = {"pastel": [100, 85],"p": [25, 85], "ltg": [25, 65], "g": [25, 35], "dkg": [25, 15],"lt": [50, 80], "sf": [50, 60], "d": [50, 40], "dk": [50, 20],"s": [70, 50], "b": [75, 75], "dp": [75, 25],	"v": [90, 50],}
+		self.vars["dic_선위치_vs_번호"] = self.vars["dic_lineposition_num_forexcel"] = {"/": 6, "\\": 5, "left": 7, "top": 8, "bottom": 9, "right": 10, "inside-h": 11, "inside-v": 12, "대각선오른쪽": 6, "대각선왼쪽": 5, "왼쪽": 7, "위쪽": 8, "아래쪽": 9, "오른쪽": 10, "안쪽세로": 11, "안쪽가로": 12, }
+		self.vars["dic_선굵기_vs_번호"] = self.vars["excel_line_thickness_dic"] = {"-": -4115, "-.": 4, "-..": 5, ".": -4118, "=": -4119, "no": -4142, "/.": 13, "실선": 1, "점선": 2, "가는점선": 1, "굵은실선": 6, "hairline": 1, "basic": -4138, "thick": 4, "thin": 2, "t-2": 1, "t0": -4138, "t1": 4, "t-1": 2, "매우가는선": 1, "일반": -4138, "굵은선": 4, "가는선": 2, "": 1, "..": -4115, "/..": 13,}
+		self.vars["dic_선형태_vs_번호"] = self.vars["dic_linestyle_num_forexcel"] = {"basic": 1, "-": -4115, "-.": 4, "-..": 5, ".": -4118, "=": -4119, "no": -4142, "/.": 13, "실선": 1, "점선": 2, "가는점선": 1, "굵은실선": 6, }
+
+		self.vars["dic_선형태_vs_번호"] = self.vars["dic_excel_line_style_vs_value"] = {"basic": 1, "": 1, "-": 1, ".": -4118, "-.": 4, "-..": 5, "..": -4115, "=": 4119, "no": -4142, "/..": 13, }
+		self.vars["dic_색이름_영어_vs_h값"] = self.vars["dic_colorname_hnum"] =  {"red": 0, "ora": 30, "yel": 60, "gre_yel": 90, "gre": 120, "gre_cya": 150 , "cya": 180, "blu_cya": 210, "blu": 240, "blu_mag": 270, "mag": 300, "red_mag": 330, "gra": 0, "whi": 0, "bla": 0, }
+		self.vars["dic_색이름_영어_vs_h값"] = self.vars["color_name_eng_vs_h_no"] = {"red": 0, "ora": 30, "yel": 60, "gre_yel": 90, "gre": 120, "gre_cya": 150 , "cya": 180, "blu_cya": 210, "blu": 240, "blu_mag": 270, "mag": 300, "red_mag": 330, "gra": 0, "whi": 0, "bla": 0, "pin": 326, }
+		self.vars["dic_색이름_영어_vs_번호"] = self.vars["color_name_eng_vs_index"] = {"red": 0, "ora": 1, "yel": 2, "gre_yel": 3, "gre": 4, "gre_cya": 5, "cya": 6, "blu_cya": 7, "blu": 8, "blu_mag": 9, "mag": 10, "red_mag": 11, "gra": 12, "whi": 13, "bla": 14}
+		self.vars["dic_색이름_영어_vs_번호"] = self.vars["dic_color_name_eng_vs_color_index"] = {"red": 0, "ora": 1, "yel": 2, "yg": 3, "gre": 4, "gre_cya": 5, "cya": 6, "cb": 7, "blu": 8, "blu_mag": 9, "mag": 10, "mr": 11, "gra": 12, "whi": 13, "bla": 14}
+		self.vars["dic_sl값_큰단계_vs_sl값"] = self.vars["dic_num_slstep"] =  {"1": [100, 80], "2": [100, 77], "3": [100, 68], "4": [100, 59],"5": [100, 50], "6": [90, 41], "7": [80, 32], "8": [70, 23], "9": [60, 14] }
+		self.vars["dic_sl값_작은단계_vs_sl값"] = self.vars["dic_num_slstep_small"] =  {"1": [0, 12], "2": [0, 9], "3": [0, 6], "4": [0, 3],"5": [0, 0], "6": [0, -3], "7": [0, -6], "8": [0, -9], "9": [0, -12], "0": [0, -14], }
+		self.vars["dic_월이름_영어_vs_번호"] = self.vars["mon_eng_vs_no"] = {"JAN":1, "FEB":2, "MAR":3, "APR":4, "MAY":5, "JUN":6, "JUL":7, "AUG":8, "SEP":9, "OCT":10, "NOV":11, "DEC":12, "JANUARY":1, "FEBRUARY":2, "MARCH":3, "APRIL":4, "JUNE":6, "JULY":7, "AUGUST":8,"SEPTEMBER":9, "OCTOBER":10, "NOVEMBER":11, "DECEMBER":12}
+		self.vars["dic_색강도_vs_sl값"] = self.vars["+-_value_vs_sl_no"] = {"+++++": [0, 15], "++++": [0, 12], "+++": [0, 9], "++": [0, 6], "+": [0, 3], "-": [0, -3],"--": [0, -6], "---": [0, -9], "----": [0, -12], "-----": [0, -14], }
+		self.vars["dic_번호_vs_s단계"] = self.vars["dic_num_sstep"] = {"1": [10], "2": [20], "3": [30], "4": [40], "5": [50], "6": [60], "7": [70], "8": [80], "9": [90], }
+		self.vars["dic_번호_vs_l단계"] = self.vars["dic_num_lstep"] = {"1": [10], "2": [20], "3": [30], "4": [40], "5": [50], "6": [60], "7": [70], "8": [80], "9": [90], }
+
+		#self.vars["dic_sl_small_step_vs_sl값"] = {"9": [0, 12], "8": [0, 9], "7": [0, 6], "6": [0, 3],	"5": [0, 0], "4": [0, -3], "3": [0, -6], "2": [0, -9], "1": [0, -12],	"0": [0, -14], }
+		#self.vars["color_name_for_all_eng"] = ['bla 0', 'whi 0', 'gra 0', 'red 0', 'ora 30', 'bro 30', 'yel 60', 'gre_yel 90', 'gre 120', 'gre_cya 150', 'sul_yel 150', 'cya 180', 'blu_cya 210', 'blu 240', 'blu_mag 270', 'mag 300', 'pal_pin 303', 'pin 326', 'red_mag 330', 'sca 343']
+		#self.vars["color_name_for_all_eng"] = list(set(self.vars["check_color_name_eng"].values()))
+		#self.vars["color_name_for_all_eng"] = ['bro 30', 'pal_pin 303', 'pin 326', 'sca 343']
+
+
+		#self.vars["dic_rgb값_vs_엑셀_색번호"] = self.vars["excel_rgblist_vs_colorindex"] = {[0, 0, 0]: 1, [255, 255, 255]: 2, [255, 0, 0]: 3, [0, 255, 0]: 4, [0, 0, 255]: 5,
+		#		 [255, 255, 0]: 6, [255, 0, 255]: 7, [0, 255, 255]: 8, [128, 0, 0]: 9, [0, 128, 0]: 10,
+		#		 [0, 0, 128]: 11, [128, 128, 0]: 12, [128, 0, 128]: 13, [0, 128, 128]: 14, [192, 192, 192]: 15,
+		#		 [128, 128, 128]: 16, [153, 153, 255]: 17, [153, 51, 102]: 18, [255, 255, 204]: 19, [204, 255, 255]: 20,
+		#		 [102, 0, 102]: 21, [255, 128, 128]: 22, [0, 102, 204]: 23, [204, 204, 255]: 24, [0, 0, 128]: 25,
+		#		 [255, 0, 255]: 26, [255, 255, 0]: 27, [0, 255, 255]: 28, [128, 0, 128]: 29, [128, 0, 0]: 30,
+		#		 [0, 128, 128]: 31, [0, 0, 255]: 32, [0, 204, 255]: 33, [204, 255, 255]: 34, [204, 255, 204]: 35,
+		#		 [255, 255, 153]: 36, [153, 204, 255]: 37, [255, 153, 204]: 38, [204, 153, 255]: 39,
+		#		 [255, 204, 153]: 40,
+		#		 [51, 102, 255]: 41, [51, 204, 204]: 42, [153, 204, 0]: 43, [255, 204, 0]: 44, [255, 153, 0]: 45,
+		#		 [255, 102, 0]: 46, [102, 102, 153]: 47, [150, 150, 150]: 48, [0, 51, 102]: 49, [51, 153, 102]: 50,
+		#		 [0, 51, 0]: 51, [51, 51, 0]: 52, [153, 51, 0]: 53, [153, 51, 102]: 54, [51, 51, 153]: 55,
+		#		 [51, 51, 51]: 56, }
+
+
+		self.vars["keyboard_action_list_all"] =['\\t', '\\n', '\\r', ' ', '!', '"', '#', '$', '%', '&', "'", '(',
+				')', '*', '+', ',', '-', '.', '/', '0', '1', '2', '3', '4', '5', '6', '7',
+				'8', '9', ':', ';', '<', '=', '>', '?', '@', '[', '\\', ']', '^', '_', '`',
+				'a', 'b', 'c', 'd', 'e','f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o',
+				'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', '{', '|', '}', '~',
+				'accept', 'add', 'alt', 'altleft', 'altright', 'apps', 'backspace',
+				'browserback', 'browserfavorites', 'browserforward', 'browserhome',
+				'browserrefresh', 'browsersearch', 'browserstop', 'capslock', 'clear',
+				'convert', 'ctrl', 'ctrlleft', 'ctrlright', 'decimal', 'del', 'delete',
+				'divide', 'down', 'end', 'enter', 'esc', 'escape', 'execute', 'f1', 'f10',
+				'f11', 'f12', 'f13', 'f14', 'f15', 'f16', 'f17', 'f18', 'f19', 'f2', 'f20',
+				'f21', 'f22', 'f23', 'f24', 'f3', 'f4', 'f5', 'f6', 'f7', 'f8', 'f9',
+				'final', 'fn', 'hanguel', 'hangul', 'hanja', 'help', 'home', 'insert', 'junja',
+				'kana', 'kanji', 'launchapp1', 'launchapp2', 'launchmail',
+				'launchmediaselect', 'left', 'modechange', 'multiply', 'nexttrack',
+				'nonconvert', 'num0', 'num1', 'num2', 'num3', 'num4', 'num5', 'num6',
+				'num7', 'num8', 'num9', 'numlock', 'pagedown', 'pageup', 'pause', 'pgdn',
+				'pgup', 'playpause', 'prevtrack', 'print', 'printscreen', 'prntscrn',
+				'prtsc', 'prtscr', 'return', 'right', 'scrolllock', 'select', 'separator',
+				'shift', 'shiftleft', 'shiftright', 'sleep', 'space', 'stop', 'subtract', 'tab',
+				'up', 'volumedown', 'volumemute', 'volumeup', 'win', 'winleft', 'winright', 'yen',
+				'command', 'option', 'optionleft', 'optionright']
+
+
+
+		self.vars["action_key_list"] = [
+		'f1', 'f10', 'f11', 'f12', 'f2', 'f3', 'f4', 'f5', 'f6', 'f7', 'f8', 'f9',	'fn',
+		'left', 'right','up', 'down','end', 'home','space', 'tab',
+		'alt', 'altleft', 'altright', 'ctrl', 'ctrlleft', 'ctrlright','shift', 'shiftleft', 'shiftright', 'win', 'winleft', 'winright',
+		'capslock', 'del', 'delete','backspace', 'enter', 'esc', 'escape', 'insert','numlock',
+		'pagedown', 'pageup', 'pgdn', 'pgup',
+		'hanguel', 'hangul', 'hanja',
+		'printscreen', 'prtscr',
+		]
+
+
 
-		self.vars["check_color_name_eng"] = {
+		self.vars["dic_색이름_한글_vs_색이름_영어"] = self.vars["check_color_name_eng"] = self.vars["check_color_name"]={
 			"빨": "red", "적": "red", "빨강": "red", "red": "red", "r": "red", "빨간색": "red", "빨강색": "red",
 			"주": "ora", "주황": "ora", "주황색": "ora", "오렌지": "ora", "yr": "ora", "yellowred": "ora", "yellow_red": "ora", "yel_red": "ora", "yellow red": "ora", "o": "ora", "orange": "ora", "ora": "ora",
 			"노": "yel", "노랑": "yel", "노랑색": "yel", "황색": "yel", "y": "yel", "yellow": "yel", "yel": "yel",
 			"연": "gre_yel", "연두": "gre_yel", "연두색": "gre_yel", "gre_yel": "gre_yel", "gy": "gre_yel", "greenyellow": "gre_yel", "green_yellow": "gre_yel", "green yellow": "gre_yel", "green-yellow": "gre_yel", "yg": "gre_yel",
 			"초": "gre", "초록": "gre", "초록색": "gre", "g": "gre", "green": "gre", "gre": "gre", "녹색": "gre",
 			"연초록": "gre_cya", "gre_cya": "gre_cya", "greencyan": "gre_cya", "green_cyan": "gre_cya", "green cyan": "gre_cya", "cg": "gre_cya", "gc": "gre_cya",
 			"옥": "cya", "옥색": "cya", "하늘색": "cya", "하늘": "cya", "c": "cya", "cya": "cya", "cyan": "cya",
@@ -88,16 +235,17 @@
 			"검": "bla", "검정": "bla", "검정색": "bla", "흑": "bla", "흑색": "bla", "black": "bla", "bla": "bla",
 			"갈색": "bro", "brown": "bro", "bro": "bro",
 			"주홍": "sca", "sca": "sca", "scarlet": "sca", "주홍색": "sca", "선홍색": "sca", "선홍": "sca",
 			"연분홍": "pal_pin", "pale_pink": "pal_pin", "pal_pin": "pal_pin",
 			"유황색": "sul_yel", "유황": "sul_yel","sul_yel": "sul_yel",
 		}
 
-		self.vars["check_color_name_kor"] = {
-			"빨": "빨강", "적": "빨강", "red": "빨강", "r": "빨강", "빨간색": "빨강", "빨강색": "빨강",
+
+		self.vars["dic_색이름_vs_한글색이름"] = self.vars["check_color_name_kor"] = {
+			"빨": "빨강", "적": "빨강", "red": "빨강", "r": "빨강", "빨간색": "빨강", "빨강색": "빨강","빨강": "빨강",
 			"주": "오렌지", "주황": "오렌지", "주황색": "오렌지", "ora": "오렌지", "yr": "오렌지", "yellowred": "오렌지", "yellow_red": "오렌지", "yel_red": "오렌지", "yellow red": "오렌지", "o": "오렌지", "orange": "오렌지",
 			"노": "노랑", "노랑": "노랑", "노랑색": "노랑", "황색": "노랑", "y": "노랑", "yellow": "노랑", "yel": "노랑",
 			"연": "연두", "연두": "연두", "연두색": "연두", "gy": "연두", "greenyellow": "연두", "green_yellow": "연두", "gre_yel": "연두", "green yellow": "연두", "green-yellow": "연두", "yg": "연두",
 			"초": "초록", "초록": "초록", "초록색": "초록", "g": "초록", "녹색": "초록",
 			"연초록": "연초록", "greencyan": "연초록", "green_cyan": "연초록", "gre_cya": "연초록", "green cyan": "연초록", "cg": "연초록", "gc": "연초록",
 			"옥": "하늘", "옥색": "하늘", "하늘색": "하늘", "하늘": "하늘", "c": "하늘", "cya": "하늘", "cyan": "하늘",
 			"청록": "군청색", "청록색": "군청색", "청": "군청색", "군청색": "군청색", "청색": "군청색", "bluecyan": "군청색", "blue_cyan": "군청색", "blu_cya": "군청색", "blue cyan": "군청색", "cb": "군청색", "bg": "군청색", "bluegreen": "군청색",
@@ -111,43 +259,23 @@
 			"검": "검정", "검정": "검정", "검정색": "검정", "흑": "검정", "흑색": "검정", "black": "검정", "bla": "검정",
 			"갈색": "갈색", "brown": "갈색", "bro": "갈색",
 			"주홍": "주홍", "scarlet": "주홍","sca": "주홍", "주홍색": "주홍", "선홍색": "주홍", "선홍": "주홍",
 			"연분홍": "연분홍", "pale_pink": "연분홍","pal_pin": "연분홍",
 			"유황색": "유황", "유황": "유황","sulphur_yellow": "유황","sul_yel": "유황",
 		}
 
-		self.vars["check_color_name"] = self.vars["check_color_name_eng"]
-
-		self.vars["color_name_for_basic_12_eng"] = ['red', 'ora', 'yel', 'gre_yel', 'gre', 'gre_cya', 'cya', 'blu_cya', 'blu', 'blu_mag', 'pin', 'red_mag']
-		#self.vars["color_name_for_all_eng"] = ['bla 0', 'whi 0', 'gra 0', 'red 0', 'ora 30', 'bro 30', 'yel 60', 'gre_yel 90', 'gre 120', 'gre_cya 150', 'sul_yel 150', 'cya 180', 'blu_cya 210', 'blu 240', 'blu_mag 270', 'mag 300', 'pal_pin 303', 'pin 326', 'red_mag 330', 'sca 343']
-		self.vars["color_name_for_all_eng"] = list(set(self.vars["check_color_name_eng"].values()))
-
-		self.vars["color_name_for_basic_12_kor"] = ['빨강', '오렌지', '노랑', '연두', '초록', '연초록', '하늘', '군청색', '파랑', '남색', '핑크', '자주']
-		self.vars["color_name_for_all_kor"] = list(set(self.vars["check_color_name_kor"].values()))
-
-
-
-		#self.vars["color_name_for_all_eng"] = ['bro 30', 'pal_pin 303', 'pin 326', 'sca 343']
-
-		self.vars["color_name_eng_vs_h_no"] = {"red": 0, "ora": 30, "yel": 60, "gre_yel": 90, "gre": 120, "gre_cya": 150 , "cya": 180, "blu_cya": 210, "blu": 240, "blu_mag": 270, "mag": 300, "red_mag": 330, "gra": 0, "whi": 0, "bla": 0, "pin": 326, }
-		self.vars["color_name_eng_vs_index"] = {"red": 0, "ora": 1, "yel": 2, "gre_yel": 3, "gre": 4, "gre_cya": 5, "cya": 6, "blu_cya": 7, "blu": 8, "blu_mag": 9, "mag": 10, "red_mag": 11, "gra": 12, "whi": 13, "bla": 14}
-		self.vars["color_name_eng_vs_hsl_no"] = {
+		self.vars["dic_색이름_영어_vs_기본_hsl_값"] = self.vars["color_name_eng_vs_hsl_no"] = {
 			"gra": [0, 0, 50], 	"whi": [0, 0, 100], "bla": [0, 0, 0], 	"red": [0, 100, 50],
 			"ora": [30, 100, 50], "yel": [60, 100, 50], "gre_yel": [90, 100, 50], 	"gre": [120, 100, 50],
 			"gre_cya": [150, 100, 50], "cya": [180, 100, 50], "blu_cya": [210, 100, 50], "blu": [240, 100, 50],
 			"blu_mag": [270, 100, 50], "mag": [300, 100, 50], "red_mag": [330, 100, 50], "pin": [326, 75, 56],
 			"bro": [30, 100, 40], "sca": [181, 0, 16],	"pal_pin": [348, 95, 84],	"sul_yel": [150, 75, 0],
 		}
 
-		self.vars["sl_no_for_12_color_tone"] = [[90, 50], [80, 30], [80, 50], [80, 70], [50, 20], [50, 40], [50, 60], [50, 80], [20, 20], [20, 40], [20, 60], [20, 80]]
-		self.vars["color_tone_12_kor_vs_index"] = {"연한": 0, "밝은회색": 1, "회색": 2, "어두운회색": 3, "옅은": 4, "부드러운": 5, "탁한": 6, "어두운": 7, "밝은": 8, "강한": 9, "짙은": 10, "선명한": 11}
-		self.vars["color_tone_kor"] = ["연한", "밝은회색", "회색", "어두운회색", "옅은", "부드러운", "탁한", "어두운", "밝은", "강한", "짙은", "선명한"]
-		self.vars["color_tone_eng"] = ["pale", "light_grayish", "grayish", "dark_grayish", "light", "soft", "dull", "dark", "bright", "strong", "deep", "vivid"]
-		self.vars["color_tone_simple_eng_vs_sl_no"] = {"pastel": [100, 85],"p": [25, 85], "ltg": [25, 65], "g": [25, 35], "dkg": [25, 15],"lt": [50, 80], "sf": [50, 60], "d": [50, 40], "dk": [50, 20],"s": [70, 50], "b": [75, 75], "dp": [75, 25],	"v": [90, 50],}
-		self.vars["check_color_tone"] = {
+		self.vars["dic_색톤_vs_기본_색톤_영어"] = self.vars["check_color_tone"] = {
 			"파스텔": "pastel", "pastel": "pastel",
 			"p": "p", "pale": "p", "pal": "p", "연한": "p",
 			"ltg": "ltg", "light_grayish": "ltg", "gra+": "ltg", "밝은회색": "ltg",
 			"g": "g", "grayish": "g", "gra": "g", "회색": "g",
 			"dkg": "dkg", "dark_grayish": "dkg", "gra-": "dkg", "어두운회색": "dkg",
 			"lt": "lt", "light": "lt", "lig": "lt", "옅은": "lt",
 			"sf": "sf", "soft": "sf", "sof": "sf", "부드러운": "sf",
@@ -156,150 +284,75 @@
 			"b": "b", "bright": "b", "bri": "b", "밝은": "b",
 			"s": "s", "strong": "s", "str": "s", "기본": "s", "강한": "s",
 			"dp": "dp", "deep": "dp", "dee": "dp", "짙은": "dp",
 			"v": "v", "선명한": "v", "vivid": "v", "viv": "v",
 			"black": "black", "검정": "black",
 			}
 
-		self.vars["check_change_step"] = {
+		self.vars["dic_색강도_vs_기본값"] = self.vars["check_change_step"] ={
 			0: "0", "0": "0", "l5": "0", "+++++": "0", "pale": "0", "p": "0", "pastel": "0", "파스텔": "0", "d5": "0",
 			1: "1", "1": "1", "l4": "1", "++++": "1", "light_grayish": "1", "ltg": "1", "밝은회색": "1", "d4": "1",
 			2: "2", "2": "2", "l3": "2", "+++": "2", "light": "2", "lt": "2", "흐린": "2", "옅은": "2", "d3": "2",
 			3: "3", "3": "3", "l2": "3", "++": "3", "soft": "3", "sf": "3", "부드러운": "3", "d2": "3",
 			4: "4", "4": "4", "l1": "4", "+": "4", "bright": "4", "b": "4", "밝은": "4", "d1": "4",
 			5: "5", "5": "5", "l0": "5", "": "5", "strong": "5", "s": "5", "강한": "5", "d0": "5",
 			6: "6", "6": "6", "l-1": "6", "-": "6", "deep": "6", "dp": "6", "진한": "6", "d-1": "6",
 			7: "7", "7": "7", "l-2": "7", "--": "7", "dull": "7", "d": "7", "탁한": "7", "d-2": "7",
 			8: "8", "8": "8", "l-3": "8", "---": "8", "dark": "8", "dk": "8", "어두운": "8", "d-3": "8",
 			9: "9", "9": "9", "l-4": "9", "----": "9", "grayish": "9", "g": "9", "회색": "9", "잿빛": "9", "d-4": "9",
 			10: "10", "10": "10", "l-5": "10", "-----": "10", "dark_grayish": "10", "dkg": "10", "어두운회색": "10", "d-5": "10",
 			}
 
-		self.vars["sl_big_step_vs_sl_no"] = {"1": [100, 80], "2": [100, 77], "3": [100, 68], "4": [100, 59],
-		                                         "5": [100, 50], "6": [90, 41], "7": [80, 32], "8": [70, 23], "9": [60, 14] }
-		self.vars["sl_small_step_vs_sl_no"] = {"1": [0, 12], "2": [0, 9], "3": [0, 6], "4": [0, 3],
-		                                           "5": [0, 0], "6": [0, -3], "7": [0, -6], "8": [0, -9], "9": [0, -12], "0": [0, -14], }
-		self.vars["sl_no_for_faber_style"] = [[[100, 0], [100, 50], [0, 0]], [[0, 0], [0, 75], [0, 100]],
-					[[100, 0], [25, 75], [0, 100]], [[25, 0], [10, 50], [0, 75]],
-					[[100, 0], [0, 0], [0, 100]], [[25, 0], [10, 50], [0, 75], [25, 75]], ]
-		self.vars["sl_no_for_basic_10"] = [[100, 0], [90, 10], [80, 20], [70, 30], [60, 40], [50, 50], [40, 60], [30, 70], [10, 80], [10, 90], [0, 100]]
-		self.vars["sl_no_for_basic_11"] = [[100, 0], [100, 10], [100, 20], [100, 30], [100, 40], [100, 50], [100, 60], [100, 70], [100, 80], [100, 90], [100, 100]]
-		self.vars["sl_small_step_vs_sl_no"] = self.sLstep_small = {"9": [0, 12], "8": [0, 9], "7": [0, 6], "6": [0, 3],
-																	"5": [0, 0], "4": [0, -3], "3": [0, -6], "2": [0, -9], "1": [0, -12],
-																	"0": [0, -14], }
-
-		self.vars["hsl_no_for_basic_12"] = [[0, 100, 50], [30, 100, 50], [60, 100, 50], [90, 100, 50], [120, 100, 50],
-										 [150, 100, 50], [180, 100, 50], [210, 100, 50], [240, 100, 50], [270, 100, 50],
-										 [300, 100, 50], [330, 100, 50]]
 
-		self.vars["hsl_no_for_johannes_style"] = [
-			[[0, 100, 0], [0, 100, 10], [0, 100, 20], [0, 100, 30], [0, 100, 40], [0, 100, 50], [0, 100, 60], [0, 100, 70],
-			 [0, 100, 80], [0, 100, 90], [0, 100, 100]],
-			[[30, 100, 0], [30, 100, 10], [30, 100, 20], [30, 100, 30], [30, 100, 40], [30, 100, 50], [30, 100, 60],
-			 [30, 100, 70], [30, 100, 80], [30, 100, 90], [30, 100, 100]],
-			[[60, 100, 0], [60, 100, 10], [60, 100, 20], [60, 100, 30], [60, 100, 40], [60, 100, 50], [60, 100, 60],
-			 [60, 100, 70], [60, 100, 80], [60, 100, 90], [60, 100, 100]],
-			[[90, 100, 0], [90, 100, 10], [90, 100, 20], [90, 100, 30], [90, 100, 40], [90, 100, 50], [90, 100, 60],
-			 [90, 100, 70], [90, 100, 80], [90, 100, 90], [90, 100, 100]],
-			[[120, 100, 0], [120, 100, 10], [120, 100, 20], [120, 100, 30], [120, 100, 40], [120, 100, 50], [120, 100, 60],
-			 [120, 100, 70], [120, 100, 80], [120, 100, 90], [120, 100, 100]],
-			[[150, 100, 0], [150, 100, 10], [150, 100, 20], [150, 100, 30], [150, 100, 40], [150, 100, 50], [150, 100, 60],
-			 [150, 100, 70], [150, 100, 80], [150, 100, 90], [150, 100, 100]],
-			[[180, 100, 0], [180, 100, 10], [180, 100, 20], [180, 100, 30], [180, 100, 40], [180, 100, 50], [180, 100, 60],
-			 [180, 100, 70], [180, 100, 80], [180, 100, 90], [180, 100, 100]],
-			[[210, 100, 0], [210, 100, 10], [210, 100, 20], [210, 100, 30], [210, 100, 40], [210, 100, 50], [210, 100, 60],
-			 [210, 100, 70], [210, 100, 80], [210, 100, 90], [210, 100, 100]],
-			[[240, 100, 0], [240, 100, 10], [240, 100, 20], [240, 100, 30], [240, 100, 40], [240, 100, 50], [240, 100, 60],
-			 [240, 100, 70], [240, 100, 80], [240, 100, 90], [240, 100, 100]],
-			[[270, 100, 0], [270, 100, 10], [270, 100, 20], [270, 100, 30], [270, 100, 40], [270, 100, 50], [270, 100, 60],
-			 [270, 100, 70], [270, 100, 80], [270, 100, 90], [270, 100, 100]],
-			[[300, 100, 0], [300, 100, 10], [300, 100, 20], [300, 100, 30], [300, 100, 40], [300, 100, 50], [300, 100, 60],
-			 [300, 100, 70], [300, 100, 80], [300, 100, 90], [300, 100, 100]],
-			[[330, 100, 0], [330, 100, 10], [330, 100, 20], [330, 100, 30], [330, 100, 40], [330, 100, 50], [330, 100, 60],
-			 [330, 100, 70], [330, 100, 80], [330, 100, 90], [330, 100, 100]]]
-
-		self.vars["rgb_46_for_excel"] = [[255, 0, 0], [0, 255, 0], [0, 0, 255], [255, 255, 0], [255, 0, 255],
+		self.vars["list_엑셀46개_rgb값"] = self.vars["list_46rgb_forexcel"] = [[255, 0, 0], [0, 255, 0], [0, 0, 255], [255, 255, 0], [255, 0, 255],
 					 [0, 255, 255], [153, 51, 102], [255, 255, 204], [204, 255, 255], [102, 0, 102],
 					 [255, 128, 128], [0, 102, 204], [204, 204, 255], [0, 204, 255], [204, 255, 204],
 					 [255, 255, 153], [153, 204, 255], [255, 153, 204], [204, 153, 255], [255, 204, 153],
 					 [51, 102, 255], [51, 204, 204], [153, 204, 0], [255, 204, 0], [255, 153, 0],
 					 [255, 102, 0], [102, 102, 153], [150, 150, 150], [0, 51, 102], [51, 153, 102],
 					 [0, 51, 0], [51, 51, 0], [153, 51, 0], [51, 51, 153], [51, 51, 51],
 					 [128, 0, 0], [0, 128, 0], [0, 0, 128], [128, 128, 0], [128, 0, 128],
 					 [0, 128, 128], [192, 192, 192], [128, 128, 128], [153, 153, 255], [0, 0, 0],
 					 [255, 255, 255]]
 
-		self.vars["rgb_for_basic_12"] = [[255, 0, 0], [255, 128, 0], [255, 255, 0], [128, 255, 0],
-										[0, 255, 0], [0, 255, 128], [0, 255, 255], [0, 128, 255],
-										[0, 0, 255], [128, 0, 255], [255, 0, 255], [255, 0, 128], ]
 
-		self.vars["excel_colorindex_vs_rgb_no"] = {
+		self.vars["dic_엑셀_56가지_색번호_vs_rgb값"] = self.vars["list_56rgb_forexcel"] =  {
 			1: [0, 0, 0], 2: [255, 255, 255], 3: [255, 0, 0], 4: [0, 255, 0], 5: [0, 0, 255],
 			6: [255, 255, 0], 7: [255, 0, 255], 8: [0, 255, 255], 9: [128, 0, 0], 10: [0, 128, 0],
 			11: [0, 0, 128], 12: [128, 128, 0], 13: [128, 0, 128], 14: [0, 128, 128], 15: [192, 192, 192],
 			16: [128, 128, 128], 17: [153, 153, 255], 18: [153, 51, 102], 19: [255, 255, 204], 20: [204, 255, 255],
 			21: [102, 0, 102], 22: [255, 128, 128], 23: [0, 102, 204], 24: [204, 204, 255], 25: [0, 0, 128],
 			26: [255, 0, 255], 27: [255, 255, 0], 28: [0, 255, 255], 29: [128, 0, 128], 30: [128, 0, 0],
 			31: [0, 128, 128], 32: [0, 0, 255], 33: [0, 204, 255], 34: [204, 255, 255], 35: [204, 255, 204],
 			36: [255, 255, 153], 37: [153, 204, 255], 38: [255, 153, 204], 39: [204, 153, 255], 40: [255, 204, 153],
 			41: [51, 102, 255], 42: [51, 204, 204], 43: [153, 204, 0], 44: [255, 204, 0], 45: [255, 153, 0],
 			46: [255, 102, 0], 47: [102, 102, 153], 48: [150, 150, 150], 49: [0, 51, 102], 50: [51, 153, 102],
 			51: [0, 51, 0], 52: [51, 51, 0], 53: [153, 51, 0], 54: [153, 51, 102], 55: [51, 51, 153],
 			56: [51, 51, 51], }
 
-		self.vars["rgb_56_for_excel"] = []
-		self.vars["excel_colorindex_vs_rgbint"] = {}
-		for key in self.vars["excel_colorindex_vs_rgb_no"].keys():
-			value = self.vars["excel_colorindex_vs_rgb_no"][key]
-			self.vars["rgb_56_for_excel"].append(value)
-			self.vars["excel_colorindex_vs_rgbint"][value[0]*256*256 +value[1]*256 + value[2]] = key
+		#self.vars["rgb_56_for_excel"] = []
+		#self.vars["excel_colorindex_vs_rgbint"] = {}
+		#for key in self.vars["excel_colorindex_vs_rgb_no"].keys():
+		#	value = self.vars["excel_colorindex_vs_rgb_no"][key]
+		#	self.vars["rgb_56_for_excel"].append(value)
+		#	self.vars["excel_colorindex_vs_rgbint"][value[0]*256*256 +value[1]*256 + value[2]] = key
 
 
-		self.vars["excel_colorindex_vs_color_name"] = {
+		self.vars["dic_엑셀_색번호_vs_색이름"] = self.vars["excel_colorindex_vs_color_name"] = {
 			1: "검정색", 	2: "흰색", 3: "빨강색", 5: "파랑색", 6: "노랑색",
 			7: "핑크색", 46: "오렌지", 13: "보라색", 14: "청록색", 19: "옅은노랑",
 			20: "옅은하늘", 18: "매실색", 8: "밝은하늘", 4: "연두색", 15: "회색20",
 			48: "회색40", 16: "회색60", 56: "회색80", 9: "진한적색", 10: "진한녹색",
 			11: "진한청색", 12: "진한황색", 21: "진한보라", 33: "진한하늘", 49: "진한산호색",
 			17: "담자색", 45: "토황색", 35: "취람색", 36: "송화색", 40: "두록색",
 			22: "주색", 23: "청현색", 24: "회보라색", 37: "밝은벽청색", 38: "선홍색", 47: "치색",
 		}
 
-		self.vars["+-_value_vs_sl_no"] = {"+++++": [0, 15], "++++": [0, 12], "+++": [0, 9], "++": [0, 6], "+": [0, 3], "-": [0, -3],
-					"--": [0, -6], "---": [0, -9], "----": [0, -12], "-----": [0, -14], }
-		self.vars["h_no_for_basic_12"] =[0, 30, 60, 90, 120, 150, 180, 210, 240, 270, 300, 330]
-		self.vars["excel_line_style_dic"] = {
-		                                     "basic": 1, "": 1, "-": 1,
-		                                     ".": -4118, "-.": 4, "-..": 5,
-		                                     "..": -4115, "=": 4119, "no": -4142, "/..": 13, }
-		self.vars["excel_line_thickness_dic"] = {
-			"-1": 1, "매우가는선": 1, "0": 2, "": 2, "basic": 2, "가는선": 2,
-			"1": -4138, "일반선": 4138, "2": 4, "굵은선": 4,
-			"4": 1, "5": 2, "6": -4138, "7": 4,
-			"실선": -4138, "진한선": 4,}
-
-		self.vars["excel_line_position"] = {
-		                                    "l": [7], "left": [7], "왼쪽": [7],
-		                                    "t": [8], "top": [8], "위쪽": [8],
-		                                    "b": [9], "bottom": [9], "아래쪽": [9],
-		                                    "r": [10], "right": [10], "오른쪽": [10],
-		                                    "h": [11], "inside-h": [11], "inh": [11], "안쪽세로": [11], "|": [11],
-		                                    "v": [12], "inside-v": [12], "inv": [12], "안쪽가로": [12], "-": [12],
-		                                    "a": [7, 8, 9, 10, 11, 12], "all": [7, 8, 9, 10, 11, 12],
-		                                    "전부": [7, 8, 9, 10, 11, 12],
-		                                    "o": [7, 8, 9, 10], "테두리": [7, 8, 9, 10], "": [7, 8, 9, 10],
-		                                    "basic": [7, 8, 9, 10],
-		                                    "out": [7, 8, 9, 10],
-		                                    "/": [6], "대각선오른쪽": [6],
-		                                    "\\": [5], "대각선왼쪽": [5],
-		                                    "in": [11, 12],
-		                                    "total": [5, 6, 7, 8, 9, 10, 11, 12],
-		                 }
 
-		self.vars["excel_colorname_vs_colorindex"] = {
+		self.vars["dic_색이름_vs_엑셀_색번호"] = self.vars["excel_colorname_vs_colorindex"] = {
 			"bla": 1, "whi": 2, "blu": 5, "yel": 6,
 			"pin": 7, "ora": 46, "pur": 13, "gre": 14, "gra": 15,
 			"검정색": 1, "흰색": 2, "빨강색": 3, "파랑색": 5, "노랑색": 6,
 			"핑크색": 7, "오렌지": 46, "보라색": 13, "청록색": 14, "옅은노랑": 19,
 			"옅은하늘": 20, "매실색": 18, "밝은하늘": 8, "연두색": 4, "회색20": 15,
 			"회색40": 48, "회색60": 16, "회색80": 56, "진한적색": 9, "진한녹색": 10,
 			"진한청색": 11, "진한황색": 12, "진한보라": 21, "진한하늘": 33, "진한산호색": 49,
@@ -307,36 +360,22 @@
 			"주색": 22, "청현색": 23, "회보라색": 24, "밝은벽청색": 37, "선홍색": 38, "치색": 47,
 			"black": 1, "white": 2, "red": 3, "blue": 5, "yellow": 6,
 			"pink": 7, "orange": 46, "purple": 13, "green": 14, "gray": 15,
 			1: "bla", 2: "whi", 5: "blu", 6: "yel",
 			7: "pin", 46: "ora", 13: "pur", 14: "gre", 15: "gra",
 		}
 
-		#self.vars["excel_rgblist_vs_colorindex"] = {[0, 0, 0]: 1, [255, 255, 255]: 2, [255, 0, 0]: 3, [0, 255, 0]: 4, [0, 0, 255]: 5,
-		#		 [255, 255, 0]: 6, [255, 0, 255]: 7, [0, 255, 255]: 8, [128, 0, 0]: 9, [0, 128, 0]: 10,
-		#		 [0, 0, 128]: 11, [128, 128, 0]: 12, [128, 0, 128]: 13, [0, 128, 128]: 14, [192, 192, 192]: 15,
-		#		 [128, 128, 128]: 16, [153, 153, 255]: 17, [153, 51, 102]: 18, [255, 255, 204]: 19, [204, 255, 255]: 20,
-		#		 [102, 0, 102]: 21, [255, 128, 128]: 22, [0, 102, 204]: 23, [204, 204, 255]: 24, [0, 0, 128]: 25,
-		#		 [255, 0, 255]: 26, [255, 255, 0]: 27, [0, 255, 255]: 28, [128, 0, 128]: 29, [128, 0, 0]: 30,
-		#		 [0, 128, 128]: 31, [0, 0, 255]: 32, [0, 204, 255]: 33, [204, 255, 255]: 34, [204, 255, 204]: 35,
-		#		 [255, 255, 153]: 36, [153, 204, 255]: 37, [255, 153, 204]: 38, [204, 153, 255]: 39,
-		#		 [255, 204, 153]: 40,
-		#		 [51, 102, 255]: 41, [51, 204, 204]: 42, [153, 204, 0]: 43, [255, 204, 0]: 44, [255, 153, 0]: 45,
-		#		 [255, 102, 0]: 46, [102, 102, 153]: 47, [150, 150, 150]: 48, [0, 51, 102]: 49, [51, 153, 102]: 50,
-		#		 [0, 51, 0]: 51, [51, 51, 0]: 52, [153, 51, 0]: 53, [153, 51, 102]: 54, [51, 51, 153]: 55,
-		#		 [51, 51, 51]: 56, }
-
 		#기본 색스타일을 기본스타일로 변경하는 것이다
-		self.vars["dic_check_colorstyle"] = {"v": "v", "b": "b", "s": "s", "dp": "dp", "lt": "lt", "sf": "sf", "d": "d", "dk": "dk", "p": "p", "ltg": "ltg", "g": "g", "dkg": "dkg",
+		self.vars["dic_색스타일_vs_기본_색스타일"] = self.vars["dic_check_colorstyle"] = {"v": "v", "b": "b", "s": "s", "dp": "dp", "lt": "lt", "sf": "sf", "d": "d", "dk": "dk", "p": "p", "ltg": "ltg", "g": "g", "dkg": "dkg",
 				"vivid": "v", "bright": "b", "strong": "s", "deep": "dp", "light": "lt", "soft": "sf", "dull": "d", "dark": "dk", "pale": "p", "lightgrayish": "ltg", "grayish": "g", "darkgrayish": "dkg",
 				"viv": "v", "bri": "b", "str": "s", "dee": "dp", "lig": "lt", "sof": "sf", "dul": "d", "dar": "dk", "pal": "p", "gra+": "ltg", "gra": "g", "gra-": "dkg",
 				"선명한": "v", "밝은": "b", "강한": "s", "짙은": "dp", "옅은": "lt", "부드러운": "sf", "둔한": "d", "어두운": "dk", "연한": "p", "밝은회색조": "ltg", "회색조": "g", "어두운회색조": "dkg"}
 
 		#자주 사용하는 색의 이름을 기본색 이름으로 변경하는 것이다
-		self.vars["dic_check_colorname"] = {
+		self.vars["dic_색이름_vs_기본_영어_색이름"] = self.vars["dic_check_colorname"] = {
 			"빨": "red", "적": "red", "red": "red", "r": "red", "빨강": "red", 0: "red",
 			"주": "ora", "yr": "ora", "yellowred": "ora", "o": "ora", "orange": "ora", "ora": "ora", "주황": "ora", 1: "ora", 30: "ora",
 			"노": "yel", "y": "yel", "yellow": "yel", "yel": "yel", "노랑": "yel", 2: "yel", 60: "yel",
 			"연": "gre_yel", "gre_yel": "gre_yel", "greenyellow": "gre_yel", "연두": "gre_yel", "green-yellow": "gre_yel", "yg": "gre_yel", 3: "gre_yel", 90: "gre_yel",
 			"초": "gre", "g": "gre", "green": "gre", "gre": "gre", "녹색": "gre", "초록": "gre", 4: "gre", 120: "gre",
 			"연초록": "gre_cya", "green-cyan": "gre_cya", "cg": "gre_cya", "gc": "gre_cya", 5: "gre_cya", 150: "gre_cya",
 			"옥": "cya", "옥색": "cya", "c": "cya", "cya": "cya", "cyan": "cya", 6: "cya", 180: "cya",
@@ -347,182 +386,79 @@
 			"자홍": "red_mag", "red-magenta": "red_mag", "red_mag": "red_mag", "red_magenta": "red_mag", "mr": "red_mag", "자주": "red_mag", 11: "red_mag", 330: "red_mag",
 			"회": "gra", "회색": "gra", "gra": "gra", "gray": "gra", 12: "gra",
 			"흰": "whi", "하양": "whi", "white": "whi", "whi": "whi", "흰색": "whi", 13: "whi",
 			"검": "bla", "검정": "bla", "black": "bla", "흑": "bla", "bla": "bla", 14: "bla",
 			}
 
 		#컬러의 강도를 확인하는것
-		self.vars["dic_check_colorstrong"] = {
+		self.vars["dic_색강도_vs_기본값"] = self.vars["dic_colorname_colornum_forexcel"] = {
 			55: "55", "55": "55", "ls": "55", "strong": "55", "s": "55", "강한": "55", "기준": "55",
 			0: "0", "0": "0", "l5": "0", "+++++": "0", "pale": "0", "p": "0", "pastel": "0", "파스텔": "0", "d5": "0",
 			1: "1", "1": "1", "l4": "1", "++++": "1", "light grayish": "1", "ltg": "1", "d4": "1",
 			2: "2", "2": "2", "l3": "2", "+++": "2", "light": "2", "lt": "2", "흐린": "2", "가벼운": "2", "d3": "2",
 			3: "3", "3": "3", "l2": "3", "++": "3", "soft": "3", "sf": "3", "연한": "3", "d2": "3",
 			4: "4", "4": "4", "l1": "4", "+": "4", "bright": "4", "b": "4", "밝은": "4", "d1": "4",
 			5: "5", "5": "5", "l0": "5", "": "5", "vivid": "5", "v": "5", "선명한": "5", "basic": "5", "기본": "5", "d0": "5",
 			6: "6", "6": "6", "l-1": "6", "-": "6", "deep": "6", "dp": "6", "진한": "6", "d-1": "6",
 			7: "7", "7": "7", "l-2": "7", "--": "7", "dull": "7", "d": "7", "탁한": "7", "d-2": "7",
 			8: "8", "8": "8", "l-3": "8", "---": "8", "dark": "8", "dk": "8", "어두운": "8", "d-3": "8",
 			9: "9", "9": "9", "l-4": "9", "----": "9", "grayish": "9", "g": "9", "회색빛": "9", "잿빛": "9", "d-4": "9",
 			10: "10", "10": "10", "l-5": "10", "-----": "10", "dark grayish": "10", "dkg": "10", "어두운 회색": "10", "d-5": "10",
 			}
 
-		self.vars["dic_colorname_colornum_forexcel"] = {
+		self.vars["dic_색이름_한글_vs_엑셀_색번호"] = {
 			"검정색": 1, 	"흰색": 2, "빨강색": 3, "파랑색": 5, "노랑색": 6,
 			"핑크색": 7, "오렌지": 46, "보라색": 13, "청록색": 14, "옅은노랑": 19,
 			"옅은하늘": 20, "매실색": 18, "밝은하늘": 8, "연두색": 4, "회색20": 15,
 			"회색40": 48, "회색60": 16, "회색80": 56, "진한적색": 9, "진한녹색": 10,
 			"진한청색": 11, "진한황색": 12, "진한보라": 21, "진한하늘": 33, "진한산호색": 49,
 			"담자색": 17, "토황색": 45, "취람색": 35, "송화색": 36, "두록색": 40,
 			"주색": 22, "청현색": 23, "회보라색": 24, "밝은벽청색": 37, "선홍색": 38, "치색": 47,
 			"black": 1, "white": 2, "red": 3, "blue": 5, "yellow": 6,
 			"pink": 7, "orange": 46, "purple": 13, "green": 14, "gray": 15,
 			"bla": 1, "whi": 2, "blu": 5, "yel": 6,
 			"pin": 7, "ora": 46, "pur": 13, "gre": 14, "gra": 15,
+			"검정": 1, 	"빨강": 3, "파랑": 5, "노랑": 6,
+			"핑크": 7, "보라": 13, "청록": 14, "회색": 15,
 		}
 
-		self.vars["dic_colorname_colorindex"] = {
-			"검정": 1, 	"흰색": 2, "빨강": 3, "파랑": 5, "노랑": 6,
-			"핑크": 7, "오렌지": 46, "보라": 13, "청록": 14, "회색": 15,
-			"black": 1, "white": 2, "red": 3, "blue": 5, "yellow": 6,
-			"pink": 7, "orange": 46, "purple": 13, "green": 14, "gray": 15,
-			"bla": 1, "whi": 2, "blu": 5, "yel": 6,
-			"pin": 7, "ora": 46, "pur": 13, "gre": 14, "gra": 15,
-		}
-		self.vars["dic_colorindex_rgblist"] = {
+		self.vars["dic_엑셀_색번호_vs_rgb값"] = self.vars["dic_colorindex_rgblist"] = {
 			1: [0, 0, 0], 2: [255, 255, 255], 3: [255, 0, 0], 4: [0, 255, 0], 5: [0, 0, 255],
 			6: [255, 255, 0], 7: [255, 0, 255], 8: [0, 255, 255], 9: [128, 0, 0], 10: [0, 128, 0],
 			11: [0, 0, 128], 12: [128, 128, 0], 13: [128, 0, 128], 14: [0, 128, 128], 15: [192, 192, 192],
 			16: [128, 128, 128], 17: [153, 153, 255], 18: [153, 51, 102], 19: [255, 255, 204], 20: [204, 255, 255],
 			21: [102, 0, 102], 22: [255, 128, 128], 23: [0, 102, 204], 24: [204, 204, 255], 25: [0, 0, 128],
 			26: [255, 0, 255], 27: [255, 255, 0], 28: [0, 255, 255], 29: [128, 0, 128], 30: [128, 0, 0],
 			31: [0, 128, 128], 32: [0, 0, 255], 33: [0, 204, 255], 34: [204, 255, 255], 35: [204, 255, 204],
 			36: [255, 255, 153], 37: [153, 204, 255], 38: [255, 153, 204], 39: [204, 153, 255], 40: [255, 204, 153],
 			41: [51, 102, 255], 42: [51, 204, 204], 43: [153, 204, 0], 44: [255, 204, 0], 45: [255, 153, 0],
 			46: [255, 102, 0], 47: [102, 102, 153], 48: [150, 150, 150], 49: [0, 51, 102], 50: [51, 153, 102],
 			51: [0, 51, 0], 52: [51, 51, 0], 53: [153, 51, 0], 54: [153, 51, 102], 55: [51, 51, 153],
 			56: [51, 51, 51], }
 
-		self.vars["list_46rgb_forexcel"] = [[255, 0, 0], [0, 255, 0], [0, 0, 255], [255, 255, 0], [255, 0, 255],
-					 [0, 255, 255], [153, 51, 102], [255, 255, 204], [204, 255, 255], [102, 0, 102],
-					 [255, 128, 128], [0, 102, 204], [204, 204, 255], [0, 204, 255], [204, 255, 204],
-					 [255, 255, 153], [153, 204, 255], [255, 153, 204], [204, 153, 255], [255, 204, 153],
-					 [51, 102, 255], [51, 204, 204], [153, 204, 0], [255, 204, 0], [255, 153, 0],
-					 [255, 102, 0], [102, 102, 153], [150, 150, 150], [0, 51, 102], [51, 153, 102],
-					 [0, 51, 0], [51, 51, 0], [153, 51, 0], [51, 51, 153], [51, 51, 51],
-					 [128, 0, 0], [0, 128, 0], [0, 0, 128], [128, 128, 0], [128, 0, 128],
-					 [0, 128, 128], [192, 192, 192], [128, 128, 128], [153, 153, 255], [0, 0, 0],
-					 [255, 255, 255]]
-
-
-		self.vars["dic_colornum_colorname_forexcel"] = {
-			1: "검정색", 	2: "흰색", 3: "빨강색", 5: "파랑색", 6: "노랑색",
-			7: "핑크색", 46: "오렌지", 13: "보라색", 14: "청록색", 19: "옅은노랑",
-			20: "옅은하늘", 18: "매실색", 8: "밝은하늘", 4: "연두색", 15: "회색20",
-			48: "회색40", 16: "회색60", 56: "회색80", 9: "진한적색", 10: "진한녹색",
-			11: "진한청색", 12: "진한황색", 21: "진한보라", 33: "진한하늘", 49: "진한산호색",
-			17: "담자색", 45: "토황색", 35: "취람색", 36: "송화색", 40: "두록색",
-			22: "주색", 23: "청현색", 24: "회보라색", 37: "밝은벽청색", 38: "선홍색", 47: "치색",
-		}
-
-		self.vars["dic_check_colormode"] ={1: "단색조합", "단색조합": 1, "강력한 대기효과와 넓은공간감": 1,
-							  2: "등간격 3색 조화", "등간격 3색 조화": 2, "활동적인 인상과 이미지": 2,
-							  3: "보색", "보색": 3, "강력한비교": 3,
-							  4: "인접색", "인접색": 4, "비슷한색 찾기": 4,
-							  5: "근접보색조합", "근접보색조합": 5, "보색의 강한 인상이 부담스러울때 보색의 근처에있는 색": 5,
-							  6: "고명도배색", "고명도배색": 6,
-							  7: "고명도배색+약간더 부드러운 이미지", "고명도배색+약간더 부드러운 이미지": 7,
-							  8: "중명도배색", "중명도배색": 8,
-							  9: "중명도배색+약간더 부드러운 이미지", "중명도배색+약간더 부드러운 이미지": 9,
-							  10: "저중명도배색", "저중명도배색": 10,
-							  11: "저명도배색+약간더 어두운 이미지", "저명도배색+약간더 어두운 이미지": 11,
-							  12: "명도차가 큰 배색", "명도차가 큰 배색": 12,
-							  13: "명도차가 큰 배색 + 근접보색", "명도차가 큰 배색 + 근접보색": 13,
-							  14: "고채도 배색", "고채도 배색": 14,
-							  15: "채도차가 큰 배색", "채도차가 큰 배색": 15,
-							  16: "저채도 배색", "저채도 배색": 16, "차분하고 무거운 이미지": 16,
-							  }
-
-		self.vars["dic_color_index"] = {"red": 0, "ora": 1, "yel": 2, "yg": 3, "gre": 4, "gre_cya": 5, "cya": 6, "cb": 7, "blu": 8, "blu_mag": 9, "mag": 10, "mr": 11, "gra": 12, "whi": 13, "bla": 14}
-
-
-		self.vars["dic_num_sstep"] = {"1": [10], "2": [20], "3": [30], "4": [40], "5": [50], "6": [60], "7": [70], "8": [80], "9": [90], }
-
-		self.vars["dic_num_lstep"] = {"1": [10], "2": [20], "3": [30], "4": [40], "5": [50], "6": [60], "7": [70], "8": [80], "9": [90], }
-
-		self.vars["dic_linethick_num_forexcel"] = {"hairline": 1, "basic": -4138, "thick": 4, "thin": 2, "t-2": 1, "t0": -4138, "t1": 4, "t-1": 2, "매우가는선": 1, "일반": -4138, "굵은선": 4, "가는선": 2, }
-
-		self.vars["dic_lineposition_num_forexcel"] = {"/": 6, "\\": 5, "left": 7, "top": 8, "bottom": 9, "right": 10, "inside-h": 11, "inside-v": 12, "대각선오른쪽": 6, "대각선왼쪽": 5, "왼쪽": 7, "위쪽": 8, "아래쪽": 9, "오른쪽": 10, "안쪽세로": 11, "안쪽가로": 12, }
-
-		self.vars["dic_linestyle_num_forexcel"] = {"basic": 1, "-": -4115, "-.": 4, "-..": 5, ".": -4118, "=": -4119, "no": -4142, "/.": 13, "실선": 1, "점선": 2, "가는점선": 1, "굵은실선": 6, }
-
-		self.vars["dic_colorname_hnum"] = {"red": 0, "ora": 30, "yel": 60, "gre_yel": 90, "gre": 120, "gre_cya": 150 , "cya": 180, "blu_cya": 210, "blu": 240, "blu_mag": 270, "mag": 300, "red_mag": 330, "gra": 0, "whi": 0, "bla": 0, }
-
-		self.vars["dic_num_slstep_small"] = {"1": [0, 12], "2": [0, 9], "3": [0, 6], "4": [0, 3], "5": [0, 0], "6": [0, -3], "7": [0, -6], "8": [0, -9], "9": [0, -12], "0": [0, -14], }
-		self.vars["dic_num_slstep"] = {"1": [100, 80], "2": [100, 77], "3": [100, 68], "4": [100, 59], "5": [100, 50], "6": [90, 41], "7": [80, 32], "8": [70, 23], "9": [60, 14] }
-
-
-		self.vars["list_colorname_pccs"] = ["v", "b", "s", "dp", "lt", "sf", "d", "dk", "p", "ltg", "g", "dkg"]
-
-		self.vars["list_colorname_kor"] = ["빨강", "주황", "노랑", "연두", "초록", "연초록", "옥색", "청록", "파랑", "남색", "보라", "자홍", "회색", "흰색", "검정"]
-		self.vars["list_colorname_eng"] = ["red", "ora", "yel", "gre_yel", "gre", "gre_cya", "cya", "blu_cya", "blu", "blu_mag", "mag", "red_mag", "gra", "whi", "bla"]
-		self.vars["list_colorname_eng_short"] = ["r", "o", "y", "gre_yel", "g", "gre_cya", "c", "blu_cya", "b", "blu_mag", "m", "red_mag", "g", "w", "bl"]
-
-		self.vars["list_colorstyle_eng"] = ["vivid", "bright", "strong", "deep", "light", "soft", "dull", "dark", "pale", "lightgrayish", "grayish", "darkgrayish"]
-		self.vars["list_colorstyle_kor"] = ["파스텔", "연한", "밝은", "흐린", "선명한", "기본", "탁한", "진한", "어두운", "회색", "검은", "검정"]
-		self.vars["list_colorstyle_eng"] = ["white", "pale", "light", "soft", "vivid", "dull", "deep", "dark", "black", "gray"]
-
-		self.vars["list_colorstyle_slno"] = [[90, 50], [80, 30], [80, 50], [80, 70], [50, 20], [50, 40], [50, 60], [50, 80], [20, 20], [20, 40], [20, 60], [20, 80]]
-
-		self.vars["list_colormode_kor"]= ["단색조합", "등간격 3색 조화", "보색", "인접색", "근접보색조합",
+		self.vars["list_colormode_kor"]= self.vars["list_colormode_kor"]= ["단색조합", "등간격 3색 조화", "보색", "인접색", "근접보색조합",
 							   "고명도배색", "고명도배색+약간더 부드러운 이미지",
 							   "중명도배색", "중명도배색+약간더 부드러운 이미지", "저중명도배색", "저명도배색+약간더 어두운 이미지",
 							   "명도차가 큰 배색", "명도차가 큰 배색 + 근접보색",
 							   "고채도 배색", "채도차가 큰 배색", "저채도 배색", ]
 
-		self.vars["list_56rgb_forexcel"] = [[0, 0, 0], [255, 255, 255], [255, 0, 0], [0, 255, 0], [0, 0, 255], [255, 255, 0],
+		self.vars["list_엑셀_56가지_rgb값"] = [[0, 0, 0], [255, 255, 255], [255, 0, 0], [0, 255, 0], [0, 0, 255], [255, 255, 0],
 										[255, 0, 255], [0, 255, 255], [128, 0, 0], [0, 128, 0], [0, 0, 128], [128, 128, 0],
 										[128, 0, 128], [0, 128, 128], [192, 192, 192], [128, 128, 128], [153, 153, 255],
 										[153, 51, 102], [255, 255, 204], [204, 255, 255], [102, 0, 102], [255, 128, 128],
 										[0, 102, 204], [204, 204, 255], [0, 0, 128], [255, 0, 255], [255, 255, 0],
 										[0, 255, 255], [128, 0, 128], [128, 0, 0], [0, 128, 128], [0, 0, 255],
 										[0, 204, 255], [204, 255, 255], [204, 255, 204], [255, 255, 153], [153, 204, 255],
 										[255, 153, 204], [204, 153, 255], [255, 204, 153], [51, 102, 255], [51, 204, 204],
 										[153, 204, 0], [255, 204, 0], [255, 153, 0], [255, 102, 0], [102, 102, 153],
 										[150, 150, 150], [0, 51, 102], [51, 153, 102], [0, 51, 0], [51, 51, 0],
 										[153, 51, 0], [153, 51, 102], [51, 51, 153], [51, 51, 51]]
 
-		self.vars["list_46rgb_forexcel"] = [[255, 0, 0], [0, 255, 0], [0, 0, 255], [255, 255, 0], [255, 0, 255],
-					 [0, 255, 255], [153, 51, 102], [255, 255, 204], [204, 255, 255], [102, 0, 102],
-					 [255, 128, 128], [0, 102, 204], [204, 204, 255], [0, 204, 255], [204, 255, 204],
-					 [255, 255, 153], [153, 204, 255], [255, 153, 204], [204, 153, 255], [255, 204, 153],
-					 [51, 102, 255], [51, 204, 204], [153, 204, 0], [255, 204, 0], [255, 153, 0],
-					 [255, 102, 0], [102, 102, 153], [150, 150, 150], [0, 51, 102], [51, 153, 102],
-					 [0, 51, 0], [51, 51, 0], [153, 51, 0], [51, 51, 153], [51, 51, 51],
-					 [128, 0, 0], [0, 128, 0], [0, 0, 128], [128, 128, 0], [128, 0, 128],
-					 [0, 128, 128], [192, 192, 192], [128, 128, 128], [153, 153, 255], [0, 0, 0],
-					 [255, 255, 255]]
-
-		self.vars["list_basic_12rgb"] = [[255, 0, 0], [255, 128, 0], [255, 255, 0], [128, 255, 0],
-										[0, 255, 0], [0, 255, 128], [0, 255, 255], [0, 128, 255],
-										[0, 0, 255], [128, 0, 255], [255, 0, 255], [255, 0, 128], ]
-
-		self.vars["list_basic_12hsl"] = [[0, 100, 50], [30, 100, 50], [60, 100, 50], [90, 100, 50], [120, 100, 50],
-										 [150, 100, 50], [180, 100, 50], [210, 100, 50], [240, 100, 50], [270, 100, 50],
-										 [300, 100, 50], [330, 100, 50]]
-
-		self.vars["list_basic_12h"] = [0, 30, 60, 90, 120, 150, 180, 210, 240, 270, 300, 330]
-
-		self.vars["list_basic_10sl"] = [[100, 0], [90, 10], [80, 20], [70, 30], [60, 40], [50, 50], [40, 60], [30, 70], [10, 80], [10, 90], [0, 100]]
-
-		self.vars["list_basic_11sl"] = [[100, 0], [100, 10], [100, 20], [100, 30], [100, 40], [100, 50], [100, 60], [100, 70], [100, 80], [100, 90], [100, 100]]
-
-		self.vars["list_basic_12colorstyle"] = [[90, 50], [80, 30], [80, 50], [80, 70], [50, 20], [50, 40], [50, 60], [50, 80], [20, 20], [20, 40], [20, 60], [20, 80]]
 
-		self.vars["list_johannes_hsl"] = [
+		self.vars["list_johannes의_hsl값"] = self.vars["hsl_no_for_johannes_style"] = [
 			[[0, 100, 0], [0, 100, 10], [0, 100, 20], [0, 100, 30], [0, 100, 40], [0, 100, 50], [0, 100, 60], [0, 100, 70],
 			 [0, 100, 80], [0, 100, 90], [0, 100, 100]],
 			[[30, 100, 0], [30, 100, 10], [30, 100, 20], [30, 100, 30], [30, 100, 40], [30, 100, 50], [30, 100, 60],
 			 [30, 100, 70], [30, 100, 80], [30, 100, 90], [30, 100, 100]],
 			[[60, 100, 0], [60, 100, 10], [60, 100, 20], [60, 100, 30], [60, 100, 40], [60, 100, 50], [60, 100, 60],
 			 [60, 100, 70], [60, 100, 80], [60, 100, 90], [60, 100, 100]],
 			[[90, 100, 0], [90, 100, 10], [90, 100, 20], [90, 100, 30], [90, 100, 40], [90, 100, 50], [90, 100, 60],
@@ -540,191 +476,101 @@
 			[[270, 100, 0], [270, 100, 10], [270, 100, 20], [270, 100, 30], [270, 100, 40], [270, 100, 50], [270, 100, 60],
 			 [270, 100, 70], [270, 100, 80], [270, 100, 90], [270, 100, 100]],
 			[[300, 100, 0], [300, 100, 10], [300, 100, 20], [300, 100, 30], [300, 100, 40], [300, 100, 50], [300, 100, 60],
 			 [300, 100, 70], [300, 100, 80], [300, 100, 90], [300, 100, 100]],
 			[[330, 100, 0], [330, 100, 10], [330, 100, 20], [330, 100, 30], [330, 100, 40], [330, 100, 50], [330, 100, 60],
 			 [330, 100, 70], [330, 100, 80], [330, 100, 90], [330, 100, 100]]]
 
-		self.vars["list_faber_sl"] = [[[100, 0], [100, 50], [0, 0]],
+		self.vars["list_faber의_sl값"] = self.vars["list_faber_sl"] = [[[100, 0], [100, 50], [0, 0]],
 					[[0, 0], [0, 75], [0, 100]],
 					[[100, 0], [25, 75], [0, 100]],
 					[[25, 0], [10, 50], [0, 75]],
 					[[100, 0], [0, 0], [0, 100]],
 					[[25, 0], [10, 50], [0, 75], [25, 75]], ]
 
-		self.vars["enum_line"] = {
+		self.vars["dic_엑셀_색번호_vs_색이름_한글"] = self.vars["dic_colornum_colorname_forexcel"] = {
+			1: "검정색", 	2: "흰색", 3: "빨강색", 5: "파랑색", 6: "노랑색",
+			7: "핑크색", 46: "오렌지", 13: "보라색", 14: "청록색", 19: "옅은노랑",
+			20: "옅은하늘", 18: "매실색", 8: "밝은하늘", 4: "연두색", 15: "회색20",
+			48: "회색40", 16: "회색60", 56: "회색80", 9: "진한적색", 10: "진한녹색",
+			11: "진한청색", 12: "진한황색", 21: "진한보라", 33: "진한하늘", 49: "진한산호색",
+			17: "담자색", 45: "토황색", 35: "취람색", 36: "송화색", 40: "두록색",
+			22: "주색", 23: "청현색", 24: "회보라색", 37: "밝은벽청색", 38: "선홍색", 47: "치색",
+		}
+
+		self.vars["dic_번호_vs_색변환모드"] = self.vars["dic_check_colormode"] = {1: "단색조합", "단색조합": 1, "강력한 대기효과와 넓은공간감": 1,
+							  2: "등간격 3색 조화", "등간격 3색 조화": 2, "활동적인 인상과 이미지": 2,
+							  3: "보색", "보색": 3, "강력한비교": 3,
+							  4: "인접색", "인접색": 4, "비슷한색 찾기": 4,
+							  5: "근접보색조합", "근접보색조합": 5, "보색의 강한 인상이 부담스러울때 보색의 근처에있는 색": 5,
+							  6: "고명도배색", "고명도배색": 6,
+							  7: "고명도배색+약간더 부드러운 이미지", "고명도배색+약간더 부드러운 이미지": 7,
+							  8: "중명도배색", "중명도배색": 8,
+							  9: "중명도배색+약간더 부드러운 이미지", "중명도배색+약간더 부드러운 이미지": 9,
+							  10: "저중명도배색", "저중명도배색": 10,
+							  11: "저명도배색+약간더 어두운 이미지", "저명도배색+약간더 어두운 이미지": 11,
+							  12: "명도차가 큰 배색", "명도차가 큰 배색": 12,
+							  13: "명도차가 큰 배색 + 근접보색", "명도차가 큰 배색 + 근접보색": 13,
+							  14: "고채도 배색", "고채도 배색": 14,
+							  15: "채도차가 큰 배색", "채도차가 큰 배색": 15,
+							  16: "저채도 배색", "저채도 배색": 16, "차분하고 무거운 이미지": 16,
+							  }
+
+
+		self.vars["dic_선모양_vs_index번호"] = self.vars["enum_line"] = {
 			"msoArrowheadNone": 1, "msoArrowheadTriangle": 2, "msoArrowheadOpen": 3, "msoArrowheadStealth": 4,
 			"msoArrowheadDiamond": 5, "msoArrowheadOval": 6,
 			"": 1, "<": 2, ">o": 3, ">>": 4, ">": 2, "<>": 5, "o": 6,
 			"basic": 1, "none": 1, "triangle": 2, "open": 3, "stealth": 4, "diamond": 5, "oval": 6,
 			"msoArrowheadNarrow": 1, "msoArrowheadWidthMedium": 2, "msoArrowheadWide": 3,
 			"msoArrowheadShort": 1, "msoArrowheadLengthMedium": 2, "msoArrowheadLong": 3,
 			"short": 1, "narrow": 1, "medium": 2, "long": 3, "wide": 3,
 			"-1": 1, "0": 2, "1": 3,
 			"dash": 4, "dashdot": 5, "dashdotdot": 6, "rounddot": 3, "longdash": 7, "longdashdot": 8,
 			"longdashdotdot": 9,
 			"squaredot": 2,
 			"-": 4, "-.": 5, "-..": 6, ".": 3, "--": 7, "--.": 8, "--..": 9, "ㅁ": 2,
 		}
-		self.vars["base_cell_data"] = {
+
+		self.vars["dic_선위치_vs_index번호"] = self.vars["excel_line_position"] = {
+		                                    "l": [7], "left": [7], "왼쪽": [7],
+		                                    "t": [8], "top": [8], "위쪽": [8],
+		                                    "b": [9], "bottom": [9], "아래쪽": [9],
+		                                    "r": [10], "right": [10], "오른쪽": [10],
+		                                    "h": [11], "inside-h": [11], "inh": [11], "안쪽세로": [11], "|": [11],
+		                                    "v": [12], "inside-v": [12], "inv": [12], "안쪽가로": [12], "-": [12],
+		                                    "a": [7, 8, 9, 10, 11, 12], "all": [7, 8, 9, 10, 11, 12],
+		                                    "전부": [7, 8, 9, 10, 11, 12],
+		                                    "o": [7, 8, 9, 10], "테두리": [7, 8, 9, 10], "": [7, 8, 9, 10],
+		                                    "basic": [7, 8, 9, 10],
+		                                    "out": [7, 8, 9, 10],
+		                                    "/": [6], "대각선오른쪽": [6],
+		                                    "\\": [5], "대각선왼쪽": [5],
+		                                    "in": [11, 12],
+		                                    "total": [5, 6, 7, 8, 9, 10, 11, 12],
+		                 }
+
+		self.vars["dic_base_cell_data"] = {
 			"sheet_name": "",
 			"xyxy": [100, 100, 0, 0],
 			"color": 10058239,
 			"line_style": "-.",
 			"thickness": 0.5,
 			"transparency": 0,
 			"head_style": ">",
 			"head_length": "0",
 			"head_width": "0",
 			"tail_style": ">",
 			"tail_length": "0",
 			"tail_width": "0",
 		}
 
-		self.vars["list_알파벳"] = "abcdefghijklmnopqrstuvwxyz"
-		self.vars["list_자음"] = "ㄱㄴㄷㄹㅁㅂㅅㅇㅈㅊㅋㅌㅍㅎ"
-		self.vars["list_모음"] ="ㅏㅑㅓㅕㅗㅛㅜㅠㅡㅣ"
-		self.vars["list_가나다"] = "가나다라마바사아자차카타파하"
-		self.vars["list_숫자"]= "1234567890"
-		self.vars["list_그리스문자"]= "αβγδεζήθικλμνξόπρΣτ"
-		self.vars["list_로마숫자"] = "ⅠⅡⅢⅣⅤⅥⅦⅧⅨⅩ"
-		self.vars["list_원ㄱ"] = "㉠㉡㉢㉣㉤㉥㉦㉧㉨㉩㉪㉫㉬㉭"
-		self.vars["list_원가"] = "㉮㉯㉰㉱㉲㉳㉴㉵㉶㉷㉸㉹㉺㉻"
-		self.vars["list_원a"] = "ⒶⒷⒸⒹⒺⒻⒼⒽⒾⒿⓀⓁⓂⓃⓄⓅⓆⓇⓈⓉⓊⓋⓌⓍⓎⓏ"
-		self.vars["list_원1"] ="⓪①②③④⑤⑥⑦⑧⑨⑩⑪⑫⑬⑭⑮⑯⑰⑱⑲⑳㉑㉒㉓㉔㉕㉖㉗㉘㉙㉚㉛㉜㉝㉞㉟㊱㊲㊳㊴㊵㊶㊷㊸㊹㊺㊻㊼㊽㊾㊿"
-		self.vars["list_서수"] =['1ST', '2ND', '3RD', '4TH', '5TH', '6TH', '7TH', '8TH', '9TH', '10TH', '11TH', '12TH', '13TH', '14TH', '15TH', '16TH', '17TH', '18TH', '19TH', '20TH', '21ST', '22ND', '23RD', '24TH', '25TH', '26TH', '27TH', '28TH', '29TH', '30TH', '31ST']
-
-		self.vars["list_month_eng_short"] = ['JAN', 'FEB', 'MAR', 'APR', 'MAY', 'JUN', 'JUL', 'AUG', 'SEP', 'OCT', 'NOV', 'DEC']
-		self.vars["list_month_eng"] = ['JANUARY', 'FEBRUARY', 'MARCH', 'APRIL', 'MAY', 'JUNE', 'JULY', 'AUGUST', 'SEPTEMBER', 'OCTOBER', 'NOVEMBER', 'DECEMBER']
-		self.vars["list_getdigit"] = ['one', 'two', 'three', 'four', 'five', 'six', 'seven', 'eight', 'nine']
-		self.vars["list_num_eng_00digit"] = ['twenty', 'thirty', 'forty', 'fifty', 'sixty', 'seventy', 'eighty', 'ninety']
-		self.vars["list_num_eng_10"] = ['ten', 'eleven', 'twelve', 'thirteen', 'fourteen', 'fifteen', 'sixteen', 'eighteen', 'nineteen']
-		self.vars["list_num_eng_unit_1000"] = ['thousand', 'million', 'billion', 'trillion']
-		self.vars["list_currency_eng_last"] = ['no', 'one', 'dollars']
-		self.vars["list_num_last_cent"] = ['only', 'and one cent', 'and', 'cents']
-
-		self.vars["keyboard_hex_code"] = {}
-		self.vars["keyboard_hex_code"]["VK_LBUTTON"]  = [0x01, "마우스 왼쪽 버른"]
-		self.vars["keyboard_hex_code"]["VK_RBUTTON"] = [0x02, "마우스 오른쪽 버튼"]
-		self.vars["keyboard_hex_code"]["VK_CANCEL"] = [0x03, "Ctrl+Break"]
-		self.vars["keyboard_hex_code"]["VK_MBUTTON"] = [0x04, "마우스 가운데 버튼"]
-		self.vars["keyboard_hex_code"]["VK_XBUTTON1"] = [0x05, "X1 마우스 버튼"]
-		self.vars["keyboard_hex_code"]["VK_XBUTTON2"] = [0x06, "X2 마우스 버튼"]
-		self.vars["keyboard_hex_code"]["VK_BACK"] = [0x08, "Backspace"]
-		self.vars["keyboard_hex_code"]["VK_TAB"] = [0x09, "Tab"]
-		self.vars["keyboard_hex_code"]["VK_CLEAR"] = [0x0C, "Clear 키"]
-		self.vars["keyboard_hex_code"]["VK_RETURN"] = [0x0D, "Enter"]
-		self.vars["keyboard_hex_code"]["VK_SHIFT"] = [0x10, "Shift"]
-		self.vars["keyboard_hex_code"]["VK_CONTROL"] = [0x11, "Ctrl"]
-		self.vars["keyboard_hex_code"]["VK_MENU"] = [0x12, "Alt"]
-		self.vars["keyboard_hex_code"]["VK_PAUSE"] = [0x13, "Pause"]
-		self.vars["keyboard_hex_code"]["VK_CAPITAL"] = [0x14, "Caps Lock"]
-		self.vars["keyboard_hex_code"]["VK_HANGUEL"] = [0x15, "IME 가나 모드 / 한글 모드"]
-		self.vars["keyboard_hex_code"]["VK_KANA"] = [0x15, "IME 가나 모드 / 한글 모드"]
-		self.vars["keyboard_hex_code"]["VK_JUNJA"] = [0x17, "IME 전자 모드"]
-		self.vars["keyboard_hex_code"]["VK_FINAL"] = [0x18, "IME 최종 모드"]
-		self.vars["keyboard_hex_code"]["VK_KANJI"] = [0x19, "IME 한자 모드"]
-		self.vars["keyboard_hex_code"]["VK_HANJA"] = [0x19, "IME 한자 모드"]
-		self.vars["keyboard_hex_code"]["VK_ESCAPE"] = [0x1B, "Esc"]
-		self.vars["keyboard_hex_code"]["VK_CONVERT"] = [0x1C, "IME 변환"]
-		self.vars["keyboard_hex_code"]["VK_NONCONVERT"] = [0x1D, "IME 변환 안함"]
-		self.vars["keyboard_hex_code"]["VK_ACCEPT"] = [0x1E, "IME 승인"]
-		self.vars["keyboard_hex_code"]["VK_MODECHANGE"] = [0x1F, "IME 모드 변경 요청"]
-		self.vars["keyboard_hex_code"]["VK_SPACE"] = [0x20, "Space Bar"]
-		self.vars["keyboard_hex_code"]["VK_PRIOR"] = [0x21, "Page Up"]
-		self.vars["keyboard_hex_code"]["VK_NEXT"] = [0x22, "Page Down"]
-		self.vars["keyboard_hex_code"]["VK_END"] = [0x23, "End"]
-		self.vars["keyboard_hex_code"]["VK_HOME"] = [0x24, "Home"]
-		self.vars["keyboard_hex_code"]["VK_LEFT"] = [0x25, "—"]
-		self.vars["keyboard_hex_code"]["VK_UP"] = [0x26, "?"]
-		self.vars["keyboard_hex_code"]["VK_RIGHT"] = [0x27, "-"]
-		self.vars["keyboard_hex_code"]["VK_DOWN"] = [0x28, "1"]
-		self.vars["keyboard_hex_code"]["VK_SELECT"] = [0x29, "Select"]
-		self.vars["keyboard_hex_code"]["VK_PRINT"] = [0x2A, "Print"]
-		self.vars["keyboard_hex_code"]["VK_EXECUTE"] = [0x2B, "Execute"]
-		self.vars["keyboard_hex_code"]["VK_SNAPSHOT"] = [0x2C, "Print Screen"]
-		self.vars["keyboard_hex_code"]["VK_INSERT"] = [0x2D, "Insert"]
-		self.vars["keyboard_hex_code"]["VK_DELETE"] = [0x2E, "Delete"]
-		self.vars["keyboard_hex_code"]["VK_HELP"] = [0x2F, "Help"]
-		self.vars["keyboard_hex_code"]["VK_LWIN"] = [0x5B, "왼쪽 윈도우 키"]
-		self.vars["keyboard_hex_code"]["VK_RWIN"] = [0x5C, "오른쪽 원도우 키"]
-		self.vars["keyboard_hex_code"]["VK_APPS"] = [0x5D, "어플리케이션 키"]
-		self.vars["keyboard_hex_code"]["VK_SLEEP"] = [0x5F, "Computer Sleep 키"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD0"] = [0x60, "숫자 키패드 0"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD1"] = [0x61, "숫자 키패드 1"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD2"] = [0x62, "숫자 키패드 2"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD3"] = [0x63, "숫자 키패드 3"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD4"] = [0x64, "숫자 키패드 4"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD5"] = [0x65, "숫자 키패드 5"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD6"] = [0x66, "숫자 키패드 6"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD7"] = [0x67, "숫자 키패드 7"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD8"] = [0x68, "숫자 키패드 8"]
-		self.vars["keyboard_hex_code"]["VK_NUMPAD9"] = [0x69, "숫자 키패드 9"]
-		self.vars["keyboard_hex_code"]["VK_MULTIPLY"] = [0x6A, "숫자 키패드 *"]
-		self.vars["keyboard_hex_code"]["VK_ADD"] = [0x6B, "숫자 키패드+"]
-		self.vars["keyboard_hex_code"]["VK_SEPARATOR"] = [0x6C, "Separator 키"]
-		self.vars["keyboard_hex_code"]["VK_SUBTRACT"] = [0x6D, "숫자 키패드-"]
-		self.vars["keyboard_hex_code"]["VK_DECIMAL"] = [0x6E, "숫자 키패드."]
-		self.vars["keyboard_hex_code"]["VK_DEVIDE"] = [0x6F, "숫자 키패드/"]
-		self.vars["keyboard_hex_code"]["VK_F1"] = [0x70, "F1"]
-		self.vars["keyboard_hex_code"]["VK_F2"] = [0x71, "F2"]
-		self.vars["keyboard_hex_code"]["VK_F3"] = [0x72, "F3"]
-		self.vars["keyboard_hex_code"]["VK_F4"] = [0x73, "F4"]
-		self.vars["keyboard_hex_code"]["VK_F5"] = [0x74, "F5"]
-		self.vars["keyboard_hex_code"]["VK_F6"] = [0x75, "F6"]
-		self.vars["keyboard_hex_code"]["VK_F7"] = [0x76, "F7"]
-		self.vars["keyboard_hex_code"]["VK_F8"] = [0x77, "F8"]
-		self.vars["keyboard_hex_code"]["VK_F9"] = [0x78, "F9"]
-		self.vars["keyboard_hex_code"]["VK_F10"] = [0x79, "F10"]
-		self.vars["keyboard_hex_code"]["VK_F11"] = [0x7A, "F11"]
-		self.vars["keyboard_hex_code"]["VK_F12"] = [0x7B, "F12"]
-		self.vars["keyboard_hex_code"]["VK_F13"] = [0x7C, "F13"]
-		self.vars["keyboard_hex_code"]["VK_F14"] = [0x7D, "F14"]
-		self.vars["keyboard_hex_code"]["VK_F15"] = [0x7E, "F15"]
-		self.vars["keyboard_hex_code"]["VK_F16"] = [0x7F, "F16"]
-		self.vars["keyboard_hex_code"]["VK_F17"] = [0x80, "F17"]
-		self.vars["keyboard_hex_code"]["VK_F18"] = [0x81, "F18"]
-		self.vars["keyboard_hex_code"]["VK_F19"] = [0x82, "F19"]
-		self.vars["keyboard_hex_code"]["VK_F20"] = [0x83, "F20"]
-		self.vars["keyboard_hex_code"]["VK_F21"] = [0x84, "F21"]
-		self.vars["keyboard_hex_code"]["VK_F22"] = [0x85, "F22"]
-		self.vars["keyboard_hex_code"]["VK_F23"] = [0x86, "F23"]
-		self.vars["keyboard_hex_code"]["VK_F24"] = [0x87, "F24"]
-		self.vars["keyboard_hex_code"]["VK_NUMLOCK"] = [0x90, "Num Lock"]
-		self.vars["keyboard_hex_code"]["VK_SCROLL"] = [0x91, "Scroll Lock"]
-		self.vars["keyboard_hex_code"]["VK_LSHIFT"] = [0xA0, "왼쪽 Shift"]
-		self.vars["keyboard_hex_code"]["VK_RSHIFT"] = [0xA1, "오른쪽 Shift"]
-		self.vars["keyboard_hex_code"]["VK_LCONTROL"] = [0xA2, "왼쪽 Ctrl"]
-		self.vars["keyboard_hex_code"]["VK_RCONTROL"] = [0xA3, "오른쪽 Ctrl"]
-		self.vars["keyboard_hex_code"]["VK_LMENU"] = [0xA4, "왼쪽 Alt"]
-		self.vars["keyboard_hex_code"]["VK_RMENU"] = [0xA5, "오른쪽 Alt"]
-
 
-		self.vars["first_letter"] = ["ㄱ", "ㄲ", "ㄴ", "ㄷ", "ㄸ", "ㄹ", "ㅁ", "ㅂ", "ㅃ", "ㅅ",
-		                             "ㅆ", "ㅇ", "ㅈ", "ㅉ", "ㅊ", "ㅋ", "ㅌ", "ㅍ", "ㅎ"]  # 19 글자
-		self.vars["second_letter"] = ["ㅏ", "ㅐ", "ㅑ", "ㅒ", "ㅓ", "ㅔ", "ㅕ", "ㅖ",
-		                              "ㅗ", "ㅘ", "ㅙ", "ㅚ", "ㅛ", "ㅜ", "ㅝ", "ㅞ",
-		                              "ㅟ", "ㅠ", "ㅡ", "ㅢ", "ㅣ"]  # 21 글자
-		self.vars["third_letter"] = ["", "ㄱ", "ㄲ", "ㄳ", "ㄴ", "ㄵ", "ㄶ", "ㄷ",
-		                             "ㄹ", "ㄺ", "ㄻ", "ㄼ", "ㄽ", "ㄾ", "ㄿ", "ㅀ",
-		                             "ㅁ", "ㅂ", "ㅄ", "ㅅ", "ㅆ", "ㅇ", "ㅈ", "ㅊ",
-		                             "ㅋ", "ㅌ", "ㅍ", "ㅎ"]  # 28 글자, 없는것 포함
-
-		self.vars["first_letter_no"] = {"ㄱ":0, "ㄲ":1, "ㄴ":2, "ㄷ":3, "ㄸ":4, "ㄹ":5, "ㅁ":6, "ㅂ":7, "ㅃ":8, "ㅅ":9,
-		                             "ㅆ":10, "ㅇ":11, "ㅈ":12, "ㅉ":13, "ㅊ":14, "ㅋ":15, "ㅌ":16, "ㅍ":17, "ㅎ":18}  # 19 글자
-		self.vars["second_letter_no"] = {"ㅏ":0, "ㅐ":1, "ㅑ":2, "ㅒ":3, "ㅓ":4, "ㅔ":5, "ㅕ":6, "ㅖ":7,
-		                              "ㅗ":8, "ㅘ":9, "ㅙ":10, "ㅚ":11, "ㅛ":12, "ㅜ":13, "ㅝ":14, "ㅞ":15,
-		                              "ㅟ":16, "ㅠ":17, "ㅡ":18, "ㅢ":19, "ㅣ":20}  # 21 글자
-		self.vars["third_letter_no"] = {"":0, "ㄱ":1, "ㄲ":2, "ㄳ":3, "ㄴ":4, "ㄵ":5, "ㄶ":6, "ㄷ":7,
-		                             "ㄹ":8, "ㄺ":9, "ㄻ":10, "ㄼ":11, "ㄽ":12, "ㄾ":13, "ㄿ":14, "ㅀ":15,
-		                             "ㅁ":16, "ㅂ":17, "ㅄ":18, "ㅅ":19, "ㅆ":20, "ㅇ":21, "ㅈ":22, "ㅊ":23,
-		                             "ㅋ":24, "ㅌ":25, "ㅍ":26, "ㅎ":27}  # 28 글자, 없는것 포함
 
-
-		self.vars["jamo_vs_eng"] = {
+		self.vars["dic_jamo_vs_eng"] = {
 			"ㄱ" : "a", "ㄲ" : "aa", "ㄴ" : "b", "ㄷ" : "c", "ㄸ" : "cc",
 			"ㄹ" : "d", "ㅁ" : "e", "ㅂ" : "f", "ㅃ" : "ff",
 			"ㅅ" : "g", "ㅆ" : "gg", "ㅇ" : "h", "ㅈ" : "i",
 			"ㅉ" : "ii", "ㅊ" : "j", "ㅋ" : "k", "ㅌ" : "l", "ㅍ" : "m", "ㅎ":"n",
 
 			"ㄳ" : "ag", "ㄵ" : "bi", "ㄶ" : "bn", "ㄺ" : "da",
 			"ㄻ" : "de", "ㄼ" : "df", "ㄽ" : "dg", "ㄾ" : "dl",
@@ -735,46 +581,43 @@
 			"ㅔ" : "gx", "ㅕ" : "r", "ㅖ" : "rx", "ㅗ" : "s", "ㅘ" : "so",
 			"ㅙ" : "sox", "ㅚ" : "sx", "ㅛ" : "t", "ㅜ" : "u", "ㅝ" : "ug",
 			"ㅞ" : "ugx", "ㅟ" : "ux", "ㅠ" : "v", "ㅡ" : "w", "ㅢ" : "wx", "ㅣ":"x",
 
 			"" : "", "_" : "z",
 			}
 
-		self.vars["eng_vs_jamo"] = {
+		self.vars["list_eng_vs_jamo"] = {
 			'a': 'ㄱ', 'aa': 'ㄲ', 'b': 'ㄴ', 'c': 'ㄷ', 'cc': 'ㄸ', 'd': 'ㄹ',
 			'e': 'ㅁ', 'f': 'ㅂ', 'ff': 'ㅃ', 'g': 'ㅅ', 'gg': 'ㅆ', 'h': 'ㅇ',
 			'i': 'ㅈ', 'ii': 'ㅉ', 'j': 'ㅊ', 'k': 'ㅋ', 'l': 'ㅌ', 'm': 'ㅍ',
 			'n': 'ㅎ', 'ag': 'ㄳ', 'bi': 'ㄵ', 'bn': 'ㄶ', 'da': 'ㄺ', 'de': 'ㄻ',
 			'df': 'ㄼ', 'dg': 'ㄽ', 'dl': 'ㄾ', 'dm': 'ㄿ', 'dn': 'ㅀ', 'fg': 'ㅄ',
 			'o': 'ㅏ', 'ox': 'ㅐ', 'p': 'ㅑ', 'px': 'ㅒ', 'q': 'ㅓ', 'gx': 'ㅔ',
 			'r': 'ㅕ', 'rx': 'ㅖ', 's': 'ㅗ', 'so': 'ㅘ', 'sox': 'ㅙ', 'sx': 'ㅚ',
 			't': 'ㅛ', 'u': 'ㅜ', 'ug': 'ㅝ', 'ugx': 'ㅞ', 'ux': 'ㅟ', 'v': 'ㅠ',
 			'w': 'ㅡ', 'wx': 'ㅢ', 'x': 'ㅣ', '': '', 'z': '_'}
 
-		self.vars["eng_vs_jamo_list"] = [
+		self.vars["list_eng_vs_jamo_pair"] = [
 			[['sox', 'ㅙ'], ['ugx', 'ㅞ'],],
 			[['ox', 'ㅐ'], ['px', 'ㅒ'], ['gx', 'ㅔ'], ['rx', 'ㅖ'], ['so', 'ㅘ'], ['sx', 'ㅚ'], ['wx', 'ㅢ'], ['ug', 'ㅝ'], ['ux', 'ㅟ'],],
 			[['a', 'ㄱ'],['b', 'ㄴ'],['c', 'ㄷ'], ['d', 'ㄹ'], ['e', 'ㅁ'], ['f', 'ㅂ'], ['g', 'ㅅ'], ['h', 'ㅇ'], ['i', 'ㅈ'], ['j', 'ㅊ'], ['k', 'ㅋ'], ['l', 'ㅌ'], ['m', 'ㅍ'], ['n', 'ㅎ']],
 			[['aa', 'ㄲ'], ['cc', 'ㄸ'],['ff', 'ㅃ'], ['gg', 'ㅆ'], ['ii', 'ㅉ'], ['ag', 'ㄳ'], ['bi', 'ㄵ'], ['bn', 'ㄶ'], ['da', 'ㄺ'], ['de', 'ㄻ'], ['df', 'ㄼ'], ['dg', 'ㄽ'], ['dl', 'ㄾ'], ['dm', 'ㄿ'], ['dn', 'ㅀ'], ['fg', 'ㅄ'],],
 			[['o', 'ㅏ'], ['p', 'ㅑ'], ['q', 'ㅓ'], ['r', 'ㅕ'], ['s', 'ㅗ'], ['t', 'ㅛ'], ['u', 'ㅜ'], ['v', 'ㅠ'], ['w', 'ㅡ'], ['x', 'ㅣ'],],
 		    [['z', '_']],
 			]
 
-		self.vars["mon_eng_vs_no"] = {"JAN":1, "FEB":2, "MAR":3, "APR":4, "MAY":5, "JUN":6,
-		                              "JUL":7, "AUG":8, "SEP":9, "OCT":10, "NOV":11, "DEC":12,
-		                              "JANUARY":1, "FEBRUARY":2, "MARCH":3, "APRIL":4, "JUNE":6,
-		                              "JULY":7, "AUGUST":8,"SEPTEMBER":9, "OCTOBER":10, "NOVEMBER":11, "DECEMBER":12}
 
 
-		self.vars["jfinder_gui_dic_1"] = {"탐색방법 => 최소탐색": [1, '(최소찾기)'], "탐색방법 => 최대탐색": [1, "(최대찾기)"],
+		self.vars["dic_jfinder_gui_dic_1"] = {"탐색방법 => 최소탐색": [1, '(최소찾기)'], "탐색방법 => 최대탐색": [1, "(최대찾기)"],
 		              "컴파일 방법 => 대소문자무시": [1, "(대소문자무시)"],
 		              "컴파일 방법 => 개행문자포함": [1, "(개행문자포함)"],
 		              "컴파일 방법 => 여러줄로표현": [1, "(여러줄로표현)"],
 		              }
-		self.vars["jfinder_gui_dic_2"] = {
+
+		self.vars["dic_jfinder_gui_dic_2"] = {
 			"문장 맨처음부터 맞아야함": [2, '[처음]', "type_20"],
 			"맨끝에 맞아야함": [2, '[맨끝]', "type_20"],
 			"한글": [2, '한글&', "type_21"],
 			"한글모음": [2, '한글모음&', "type_21"],
 			"한글자음": [2, '한글자음&', "type_21"],
 			"영어": [2, "영어&", "type_21"],
 			"한자": [2, "한자&", "type_21"],
@@ -790,22 +633,23 @@
 			"특정단어": [2, "[(특정단어)", "type_24"],
 			"메타문자": [2, "[\메타문자", "type_24"],
 			"특수문자": [2, '[특수문자', "type_24"],
 			"특정단어제외": [2, '[^(제외할단어)', "type_24"],
 			"또는": [2, '|', "type_25"],
 			}
 
-		self.vars["jfinder_gui_dic_3"] = {"1개": [3, ":1~1]", "type_x0"],
+		self.vars["dic_jfinder_gui_dic_3"] = {"1개": [3, ":1~1]", "type_x0"],
 		              "1개이상": [3, ":1~]", "type_x0"],
 		              "1~10개사이": [3, ":1~10]", "type_x0"],
 		              "0개이상": [3, ":0~]", "type_x0"],
 		              "0개또는1개": [3, ":0~1]", "type_x0"],
 		              "n개~m개": [3, ":n~m]", "type_x0"],
 		              }
-		self.vars["jfinder_gui_dic_4"] = {"abc중 c만 1번이상 반복되는것 찾기": [4, "abc[1~]", "type_z0"],
+
+		self.vars["dic_jfinder_gui_dic_4"] = {"abc중 c만 1번이상 반복되는것 찾기": [4, "abc[1~]", "type_z0"],
 		              "abc중 bc만 1번이상 반복되는것 찾기": [4, "a(bc)[1~]", "type_z0"],
 		              "a와 b와 c를 제외한 모든 문자와 매치": [4, "[^abc]", "type_z0"],
 		              "한글로 3~5개의 글자로 된것을 그룹명 짖기": [4, "(?P<그룹명>[한글:3~5])", "type_z0"],
 		              "a와 b사이의 모든문자 찾기": [4, "a[문자:1~]b", "type_z0"],
 		              "a또는b또는c": [4, "a[또는]b[또는]c", "type_z0"],
 		              "전방탐색 : .+(?=:) => :앞의 모든 문자": [4, ".+(?=:)", "type_z0"],
 		              "후방탐색 : (?<=\$)[0-9.]+ => $뒤의 숫자": [4, "(?<=\$)[0-9.]+", "type_z0"],
@@ -817,15 +661,15 @@
 		              "지역 전화번호 찾기": [4, "0(2|31|32|33|41|42|43|44|51|52|53|54|55|61|62|63|64)\-{0,1}\d{3,4}\-{0,1}\d{4}",
 		                             "type_z0"],
 		              "주민등록번호": [4, "[0-9]{2}0[1-9]|1[0-2]0[1-9]|[1,2][0-9]|3[0,1]-[1-4][0-9]{6}", "type_z0"],
 		              "금액": [4, "[숫자,][1~][원:0~1]", "type_z0"],
 		              "중복된 단어 찾기": [4, "\\b(\\w+)\\s+\\1\\b", "type_z0"],
 		              }
 
-		self.vars["shape_enum"] ={
+		self.vars["dic_shape_enum"] ={
 			'mixed': -2,
 			'rectangle': 1,
 			'직사각형': 1,
 			'parallelogram': 2,
 			'평행사변형': 2,
 			'trapezoid': 3,
 			'사다리꼴': 3,
@@ -1047,14 +891,113 @@
 			'Cloud': 179,
 			'ChartX': 180,
 			'ChartStar': 181,
 			'ChartPlus': 182,
 			'LineInverse': 183,}
 
 
+		self.vars["keyboard_hex_code"] = {}
+		self.vars["keyboard_hex_code"]["VK_LBUTTON"]  = [0x01, "마우스 왼쪽 버른"]
+		self.vars["keyboard_hex_code"]["VK_RBUTTON"] = [0x02, "마우스 오른쪽 버튼"]
+		self.vars["keyboard_hex_code"]["VK_CANCEL"] = [0x03, "Ctrl+Break"]
+		self.vars["keyboard_hex_code"]["VK_MBUTTON"] = [0x04, "마우스 가운데 버튼"]
+		self.vars["keyboard_hex_code"]["VK_XBUTTON1"] = [0x05, "X1 마우스 버튼"]
+		self.vars["keyboard_hex_code"]["VK_XBUTTON2"] = [0x06, "X2 마우스 버튼"]
+		self.vars["keyboard_hex_code"]["VK_BACK"] = [0x08, "Backspace"]
+		self.vars["keyboard_hex_code"]["VK_TAB"] = [0x09, "Tab"]
+		self.vars["keyboard_hex_code"]["VK_CLEAR"] = [0x0C, "Clear 키"]
+		self.vars["keyboard_hex_code"]["VK_RETURN"] = [0x0D, "Enter"]
+		self.vars["keyboard_hex_code"]["VK_SHIFT"] = [0x10, "Shift"]
+		self.vars["keyboard_hex_code"]["VK_CONTROL"] = [0x11, "Ctrl"]
+		self.vars["keyboard_hex_code"]["VK_MENU"] = [0x12, "Alt"]
+		self.vars["keyboard_hex_code"]["VK_PAUSE"] = [0x13, "Pause"]
+		self.vars["keyboard_hex_code"]["VK_CAPITAL"] = [0x14, "Caps Lock"]
+		self.vars["keyboard_hex_code"]["VK_HANGUEL"] = [0x15, "IME 가나 모드 / 한글 모드"]
+		self.vars["keyboard_hex_code"]["VK_KANA"] = [0x15, "IME 가나 모드 / 한글 모드"]
+		self.vars["keyboard_hex_code"]["VK_JUNJA"] = [0x17, "IME 전자 모드"]
+		self.vars["keyboard_hex_code"]["VK_FINAL"] = [0x18, "IME 최종 모드"]
+		self.vars["keyboard_hex_code"]["VK_KANJI"] = [0x19, "IME 한자 모드"]
+		self.vars["keyboard_hex_code"]["VK_HANJA"] = [0x19, "IME 한자 모드"]
+		self.vars["keyboard_hex_code"]["VK_ESCAPE"] = [0x1B, "Esc"]
+		self.vars["keyboard_hex_code"]["VK_CONVERT"] = [0x1C, "IME 변환"]
+		self.vars["keyboard_hex_code"]["VK_NONCONVERT"] = [0x1D, "IME 변환 안함"]
+		self.vars["keyboard_hex_code"]["VK_ACCEPT"] = [0x1E, "IME 승인"]
+		self.vars["keyboard_hex_code"]["VK_MODECHANGE"] = [0x1F, "IME 모드 변경 요청"]
+		self.vars["keyboard_hex_code"]["VK_SPACE"] = [0x20, "Space Bar"]
+		self.vars["keyboard_hex_code"]["VK_PRIOR"] = [0x21, "Page Up"]
+		self.vars["keyboard_hex_code"]["VK_NEXT"] = [0x22, "Page Down"]
+		self.vars["keyboard_hex_code"]["VK_END"] = [0x23, "End"]
+		self.vars["keyboard_hex_code"]["VK_HOME"] = [0x24, "Home"]
+		self.vars["keyboard_hex_code"]["VK_LEFT"] = [0x25, "—"]
+		self.vars["keyboard_hex_code"]["VK_UP"] = [0x26, "?"]
+		self.vars["keyboard_hex_code"]["VK_RIGHT"] = [0x27, "-"]
+		self.vars["keyboard_hex_code"]["VK_DOWN"] = [0x28, "1"]
+		self.vars["keyboard_hex_code"]["VK_SELECT"] = [0x29, "Select"]
+		self.vars["keyboard_hex_code"]["VK_PRINT"] = [0x2A, "Print"]
+		self.vars["keyboard_hex_code"]["VK_EXECUTE"] = [0x2B, "Execute"]
+		self.vars["keyboard_hex_code"]["VK_SNAPSHOT"] = [0x2C, "Print Screen"]
+		self.vars["keyboard_hex_code"]["VK_INSERT"] = [0x2D, "Insert"]
+		self.vars["keyboard_hex_code"]["VK_DELETE"] = [0x2E, "Delete"]
+		self.vars["keyboard_hex_code"]["VK_HELP"] = [0x2F, "Help"]
+		self.vars["keyboard_hex_code"]["VK_LWIN"] = [0x5B, "왼쪽 윈도우 키"]
+		self.vars["keyboard_hex_code"]["VK_RWIN"] = [0x5C, "오른쪽 원도우 키"]
+		self.vars["keyboard_hex_code"]["VK_APPS"] = [0x5D, "어플리케이션 키"]
+		self.vars["keyboard_hex_code"]["VK_SLEEP"] = [0x5F, "Computer Sleep 키"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD0"] = [0x60, "숫자 키패드 0"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD1"] = [0x61, "숫자 키패드 1"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD2"] = [0x62, "숫자 키패드 2"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD3"] = [0x63, "숫자 키패드 3"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD4"] = [0x64, "숫자 키패드 4"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD5"] = [0x65, "숫자 키패드 5"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD6"] = [0x66, "숫자 키패드 6"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD7"] = [0x67, "숫자 키패드 7"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD8"] = [0x68, "숫자 키패드 8"]
+		self.vars["keyboard_hex_code"]["VK_NUMPAD9"] = [0x69, "숫자 키패드 9"]
+		self.vars["keyboard_hex_code"]["VK_MULTIPLY"] = [0x6A, "숫자 키패드 *"]
+		self.vars["keyboard_hex_code"]["VK_ADD"] = [0x6B, "숫자 키패드+"]
+		self.vars["keyboard_hex_code"]["VK_SEPARATOR"] = [0x6C, "Separator 키"]
+		self.vars["keyboard_hex_code"]["VK_SUBTRACT"] = [0x6D, "숫자 키패드-"]
+		self.vars["keyboard_hex_code"]["VK_DECIMAL"] = [0x6E, "숫자 키패드."]
+		self.vars["keyboard_hex_code"]["VK_DEVIDE"] = [0x6F, "숫자 키패드/"]
+		self.vars["keyboard_hex_code"]["VK_F1"] = [0x70, "F1"]
+		self.vars["keyboard_hex_code"]["VK_F2"] = [0x71, "F2"]
+		self.vars["keyboard_hex_code"]["VK_F3"] = [0x72, "F3"]
+		self.vars["keyboard_hex_code"]["VK_F4"] = [0x73, "F4"]
+		self.vars["keyboard_hex_code"]["VK_F5"] = [0x74, "F5"]
+		self.vars["keyboard_hex_code"]["VK_F6"] = [0x75, "F6"]
+		self.vars["keyboard_hex_code"]["VK_F7"] = [0x76, "F7"]
+		self.vars["keyboard_hex_code"]["VK_F8"] = [0x77, "F8"]
+		self.vars["keyboard_hex_code"]["VK_F9"] = [0x78, "F9"]
+		self.vars["keyboard_hex_code"]["VK_F10"] = [0x79, "F10"]
+		self.vars["keyboard_hex_code"]["VK_F11"] = [0x7A, "F11"]
+		self.vars["keyboard_hex_code"]["VK_F12"] = [0x7B, "F12"]
+		self.vars["keyboard_hex_code"]["VK_F13"] = [0x7C, "F13"]
+		self.vars["keyboard_hex_code"]["VK_F14"] = [0x7D, "F14"]
+		self.vars["keyboard_hex_code"]["VK_F15"] = [0x7E, "F15"]
+		self.vars["keyboard_hex_code"]["VK_F16"] = [0x7F, "F16"]
+		self.vars["keyboard_hex_code"]["VK_F17"] = [0x80, "F17"]
+		self.vars["keyboard_hex_code"]["VK_F18"] = [0x81, "F18"]
+		self.vars["keyboard_hex_code"]["VK_F19"] = [0x82, "F19"]
+		self.vars["keyboard_hex_code"]["VK_F20"] = [0x83, "F20"]
+		self.vars["keyboard_hex_code"]["VK_F21"] = [0x84, "F21"]
+		self.vars["keyboard_hex_code"]["VK_F22"] = [0x85, "F22"]
+		self.vars["keyboard_hex_code"]["VK_F23"] = [0x86, "F23"]
+		self.vars["keyboard_hex_code"]["VK_F24"] = [0x87, "F24"]
+		self.vars["keyboard_hex_code"]["VK_NUMLOCK"] = [0x90, "Num Lock"]
+		self.vars["keyboard_hex_code"]["VK_SCROLL"] = [0x91, "Scroll Lock"]
+		self.vars["keyboard_hex_code"]["VK_LSHIFT"] = [0xA0, "왼쪽 Shift"]
+		self.vars["keyboard_hex_code"]["VK_RSHIFT"] = [0xA1, "오른쪽 Shift"]
+		self.vars["keyboard_hex_code"]["VK_LCONTROL"] = [0xA2, "왼쪽 Ctrl"]
+		self.vars["keyboard_hex_code"]["VK_RCONTROL"] = [0xA3, "오른쪽 Ctrl"]
+		self.vars["keyboard_hex_code"]["VK_LMENU"] = [0xA4, "왼쪽 Alt"]
+		self.vars["keyboard_hex_code"]["VK_RMENU"] = [0xA5, "오른쪽 Alt"]
+
+
+
+
 class basic_cell_class():
 	# 각 셀에대해서 어떤 자료들을 넣을수있을지 설정하도록 만든 것이다
 	# 다음에 추가적인것들도 가능하도록 클래스로 만든 것이다
 	def __init__(self):
 		self.values = {
 			"font_dic": {"font_color": None, "font_size": None, "background": None, "bold": None, "color": None, "colorindex": None, "creator": None, "style": None, "italic": None,
 				"name": None, "size": None, "strikethrough": None, "subscript": None, "superscript": None, "themecolor": None, "themefont": None, "tintandshade": None, "underline": None},
@@ -1104,14 +1047,17 @@
 			"user_1": None,
 			"user_2": None,
 			"user_3": None,
 			"x": None,
 			"y": None,
 		}
 
+
+
+
 class test_data:
 	"""
 	가끔 코딩을 해보니, 테스트용데이터가 필요하더라구요
 	입력형태 :
 	출력형태 :
 	"""
 	test_datas ={}
```

### Comparing `xython-1.3.0/src/xython/ganada.py` & `xython-1.4.0/src/xython/ganada.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 # -*- coding: utf-8 -*-
+import basic_data  # xython 모듈
+
 import win32com.client #pywin32의 모듈
-import win32
+import win32 #pywin32의 모듈
 
 class ganada:
 	"""
 	MS워드를 사용하기 쉽게하기위해 만든 모듈입니다,
 	차후에는 다른 Libero및 한글의 연동또한 만들 예정입니다
 	activedoc : 현재 선택된 워드문서
 	doc : 여러문서중에 선택한 하나의 문서
 	add : 어떤것을 만들어서 다른 조정없이 기본기능으로 새롭게 추가하는 것
 	lx : location x, 하나의 문서로 된것의 문자의 위치를 나타내는 것
 	xy : selection의 처음과 끝위치
 	xl : x는 시작위치, l은 길이
 	"""
 	def	__init__(self, file_name=""):
 		# 공통으로 사용할 변수들을 설정하는 것이다
-		self.vars = {}
+		self.base_data = basic_data.basic_data()
+		self.var = self.base_data.vars
+		self.var_common={}
+
 		self.table = ""
 		self.range = ""
 		#워드를 실행시킵니다
 		self.word_program = win32com.client.dynamic.Dispatch('Word.Application')
 		self.word_program.Visible = 1
 
 		if file_name =="":
 			#만약 오픈된 워드가 하나도 없으면,새로운 빈 워드를 만든다
 			try:
 				self.activedoc = self.word_program.ActiveDocument
 			except:
 				self.word_program.Documents.Add()
 				self.activedoc = self.word_program.ActiveDocument
-				self.selection = self.word_program.Section()
+				self.selection = self.word_program.Section
 		else:
 			self.word_program.Documents.Open(file_name)
 			self.activedoc = self.word_program.ActiveDocument
 			self.word_program.ActiveDocument.ActiveWindow.View.Type = 3
-			self.selection = self.word_program.Section()
+			self.selection = self.word_program.Section
 
 	def add_document_new(self):
 		"""
 		새 문서를 하나더 만듦
 		"""
 		self.word_program.Documents.Add()
```

### Comparing `xython-1.3.0/src/xython/jfinder.py` & `xython-1.4.0/src/xython/jfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # -*- coding: utf-8 -*-
 
 import re #내장모듈
 
 class jfinder:
+    def __init__(self):
+        # 공통으로 사용할 변수들을 설정하는 것
+        self.var_common = {}
+
+
     def manual(self):
         result = """
         1. sql을 제일 처음에, input_text를 제일 나중에
         
         """
         return result
```

### Comparing `xython-1.3.0/src/xython/mailmail.py` & `xython-1.4.0/src/xython/mailmail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 #-*- coding: utf-8 -*-
 import os #내장모듈
-import win32com.client
-import datetime
-import pynal
+import datetime #내장모듈
 
+import pynal  # xython 모듈
+import basic_data  # xython 모듈
+
+import win32com.client #pywin32의 모듈
 
 class mailmail:
     def __init__(self):
         self.base_mail = win32com.client.dynamic.Dispatch('Outlook.Application')
         self.outlook = self.base_mail.GetNamespace("MAPI")
         self.sigan = pynal.pynal()
 
+        self.base_data = basic_data.basic_data()
+        self.var = self.base_data.vars
+        self.var_common = {}
+
     def check_outlook_email_test(self):
         #테스트를 위한것
 
         outlook = win32com.client.Dispatch("Outlook.Application")
         namespace = outlook.GetNamespace("MAPI")
 
         input_folder = namespace.GetDefaultFolder(6)
@@ -510,29 +516,29 @@
         default folder: outlook 에서 기본으로 설정되고 관리되는 기준의 폴더들
         아웃룩의 메일은 item 과 folder 로 구성이 되어있다"""
         return result
 
 
     def get_mail_obj_in_mail_box_between_date(self, input_mail_box, dt_obj_from, dt_obj_to):
         #날짜사이의 메일 객체들을 갖고오는것
-        dt_obj_from = self.sigan.change_any_time_string_to_dt_obj(dt_obj_from)
-        dt_obj_to = self.sigan.change_any_time_string_to_dt_obj(dt_obj_to)
+        dt_obj_from = self.sigan.change_any_time_to_dt_obj(dt_obj_from)
+        dt_obj_to = self.sigan.change_any_time_to_dt_obj(dt_obj_to)
         #끝날묘포함하려면, 1 일을 더 더해줘야한다 #즉，2023-1-1 일 0 시 0 분 0 초를 넣어주는것과 같으므로, 2023-01-02 일 0 시 0 분 0 초로 하면 1 월 1 일의 모든 자료가 다 확인되는 것이다
         dt_obj_to = dt_obj_to + datetime.timedelta(days=1)
         #폴더객체안의 받은 날짜사이에 들어온 메세지만 갖고오는것
         messages = input_mail_box.Items
         #제일 최근에 받은즉，제일 받은시간이 늦은것을 기준으로 정렬
         messages.Sort("ReceivedTime", True)
         print(dt_obj_from.strftime("%m/%d/%Y %H:%M %p"))
         result = messages.Restrict("[ReceivedTime] >= '" + dt_obj_from.strftime("%m/%d/%Y %H:%M %p") +"' AND [ReceivedTime] 〈= '" + dt_obj_to.strftime("%m/%d/%Y %H:%M %p")+"'")
         return result
 
     def get_mail_obj_in_mail_box_from_index_day(self, input_mail_box, input_no):
         #몇일전까지의 메일을 갖고오는것
-        dt_obj_to = self.sigan.get_dt_obj_for_today()
+        dt_obj_to = self.sigan.get_today_as_dt_obj()
         #끝날포포함하려면, 1 일을 더 더해줘야한다
         #즉, 2023-1-1 일 0 시 0 분 0 초를 넣어주는것과 같으므로, 2023-01-02 일 0 시 0 분 0 초로 하면 1 월 1 일의 모든 자료가 다 확인되는 것이다
         dt_obj_from = dt_obj_to - datetime.timedelta(days=input_no-1)
         #폴더객체안의 받은 날짜사이에 들어온 메세지만 갖고오는것
         messages = input_mail_box.Items
         #제일 최근에 받은것, 즉, 제일 받은시간이 늦은것을 기준으로 정렬
         messages.Sort("ReceivedTime", True)
@@ -577,8 +583,17 @@
         new_mail = self.base_mail.CreateItem(0)
         new_mail.To = input_dic["To"]
         new_mail.Subject = input_dic["Subject"]
         new_mail.Body = input_dic["Body"]
         if "Attachments" in input_dic.keys():
             attachment = input_dic["Attachments"]
             new_mail.Attachments.Add(attachment)
-        new_mail.Send()
+        new_mail.Send()
+
+    def make_new_mail_for_draft_folder(self, **dic):
+        # 빈 임시보관함으로 보내는 메일객체를 하나 만든것
+        promise_folder = self.outlook.GetDefaultFolder(16)
+        new_mail = self.base_mail.CreateItem(0)
+        new_mail.To = dic["to"]
+        new_mail.Subject = dic["subject"]
+        new_mail.HTMubody = dic["body"]
+        new_mail.Move(promise_folder)
```

### Comparing `xython-1.3.0/src/xython/pcell.py` & `xython-1.4.0/src/xython/pcell.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # -*- coding: utf-8 -*-
 import re #내장모듈
 import os #내장모듈
 import math #내장모듈
 import string #내장모듈
 import random #내장모듈
 from itertools import combinations_with_replacement #내장모듈
+import itertools #내장모듈
 
-import scolor  # halmoney 모듈
-import basic_data  # halmoney 모듈
+import scolor  # xython 모듈
+import basic_data  # xython 모듈
 
 import win32gui #pywin32의 모듈
 import win32api #pywin32의 모듈
 import win32com.client #pywin32의 모듈
 
 class pcell:
 	"""
 	엑셀을 컨트롤 할수있는 모듈
 	"""
 	def __init__(self, filename=""):
 		#공통으로 사용할 변수들을 설정하는 것
 		self.color = scolor.scolor()
-		self.data_set_basic = basic_data.basic_data()
+		self.base_data = basic_data.basic_data()
+		self.var = self.base_data.vars
+		self.var_common={}
 		# 만약 화일의 경로가 있으면 그 화일을 열도록 한다
 		self.xlapp = win32com.client.dynamic.Dispatch('Excel.Application')
 		self.xlapp.Visible = 1
 
 		if filename != None:
 			self.filename = filename.lower()
 
@@ -46,14 +49,20 @@
 			# 만약 화일 이름이 따로 주어 지면 그 화일을 연다
 			try:
 				self.xlapp.WindowState = -4137
 				self.xlbook = self.xlapp.Workbooks.Open(self.filename)
 			except:
 				win32gui.MessageBox(0, "Please check file path", "xxw.halmoney.com", 0)
 
+	def check_basic_input_datas(self, sheet_name, xyxy):
+		if self.var["repeat_start"] and not self.var["repeat_end"] :
+			self.var["sheet_obj"] = self.check_sheet_name(sheet_name)
+			self.var["xyxy"] = self.check_address_value(xyxy)
+			self.var["my_range"] = self.var["sheet_obj"].Range(self.var["sheet_obj"].Cells(self.var["xyxy"][0], self.var["xyxy"][1]), self.var["sheet_obj"].Cells(self.var["xyxy"][2], self.var["xyxy"][3]))
+
 	def add_button_with_macro(self, sheet_name="", xyxy="", macro_code="", title=""):
 		"""
 		매크로랑 연결된 버튼을 만드는것
 		버튼을 만들어서 그 버튼에 매크로를 연결하는 것이다
 		매크로와 같은것을 특정한 버튼에 연결하여 만드는것을 보여주기위한 것이다
 		Add(왼쪽의 Pixel, 위쪽 Pixce, 넓이, 높이)
 		"""
@@ -62,14 +71,33 @@
 		new_btn = sheet_object.Buttons()
 		sheet_object.Cells(x1, y1).Select()
 		left_px, top_px, width_px, height_px = self.read_coord_in_cell("", [x1, y1])
 		new_btn.Add(left_px, top_px, width_px, height_px)
 		new_btn.OnAction = macro_code
 		new_btn.Text = title
 
+	def add_picture_in_sheet(self, sheet_name, file_path, xywh, link=0, image_in_file=1):
+		self.insert_picture_in_sheet(sheet_name, file_path, xywh, link=0, image_in_file=1)
+
+	def add_picture_in_sheet_by_pixcel(self, file_path, pxpywh, link=0, image_in_file=1):
+		vars["sheet"].Shapes.AddPicture(file_path, link, image_in_file, pxpywh[0], pxpywh[1], pxpywh[2], pxpywh[3])
+
+	def add_shape(self, sheet_name, shape_no=35, xywh=""):
+		# shape_no : 엑셀에서 정의한 도형의 번호
+		# xywh : 왼쪽윗부분의 위치에서 너비와 높이
+		sheet_object = self.check_sheet_name(sheet_name)
+
+		#도형이 숫자이면 그대로, 문자이면 기본자료에서 찾도록 한다
+		if type(shape_no) == type(123):
+			pass
+		elif shape_no in list(self.var["shape_enum"].keys()):
+			shape_no = self.var["shape_enum"][shape_no]
+
+		sheet_object.Shapes.Addshape(shape_no, xywh[0], xywh[1], xywh[2], xywh[3])
+
 	def add_sheet_new(self):
 		"""
 		시트하나 추가하기
 		위치는 자동으로 제일 뒤에 추가되는것이며, 시트이름이 없어 자동으로 만들어지는 이름입니다
 		"""
 		self.xlbook.Worksheets.Add()
 
@@ -79,29 +107,45 @@
 		위치는 자동으로 제일 뒤에 추가되는것이며, 시트이름이 없어 자동으로 만들어지는 이름입니다
 		"""
 		self.xlbook.Worksheets.Add()
 		Sheet = self.xlbook.ActiveSheet
 		if input_name != "":
 			Sheet.Name = input_name
 
+
+	def add_text_bystep(self, input_text, step):
+		#변경이 필요=================================
+		# 선택한 영역의 시작점부터 n번째 셀마다 값을 넣기
+		num = 0
+		for x in range(vars["x1"], vars["x2"] + 1):
+			for y in range(vars["y1"], vars["y2"] + 1):
+				num = num + 1
+				if divmod(num, step)[0] == 0:
+					vars["sheet"].Cells(y, x).Value = input_text
+
+
 	def add_text_in_range_at_left(self, sheet_name="", xyxy="", input_text="입력필요"):
 		"""
+		GUI : boribori에 추가됨
+		"1st": "add", "2nd": "text", "3rd": "왼쪽에 글자 추가",
+        "manual": "선택영역의 왼쪽에 글자를 추가한다",
 		선택한 영역의 왼쪽에 입력한 글자를 추가
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				cell_value = sheet_object.Cells(x, y).Value
 				if cell_value == None:
 					cell_value = ""
 				sheet_object.Cells(x, y).Value = str(input_text)+cell_value
 
 	def add_text_in_range_at_right(self, sheet_name="", xyxy="", input_text="입력필요"):
 		"""
+		GUI : boribori에 추가됨
 		선택한 영역의 오른쪽에 입력한 글자를 추가
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				cell_value = sheet_object.Cells(x, y).Value
@@ -137,14 +181,32 @@
 				for y in range(y1, y2+1):
 					if divmod(x, xystep[1])[1] == 0:
 						cell_value = sheet_object.Cells(x, y).Value
 						if cell_value == None:
 							cell_value=""
 						sheet_object.Cells(x, y).Value = cell_value+str(input_text)
 
+	def add_text_specific_string(self, check_str="", input_text=""):
+		#변경이 필요=================================
+		for x in range(vars["x1"], vars["x2"] + 1):
+			for y in range(vars["y1"], vars["y2"] + 1):
+				cell_value = vars["sheet"].Cells(y, x).Value
+				if (check_str in cell_value) and cell_value != "" and cell_value != None:
+					vars["sheet"].Cells(y, x).Value = str(input_text) + str(cell_value)
+
+
+	def change_active_workbook(self, input_file_name):
+		"""
+		열려진 워드 화일중 이름으로 선택하는것
+		"""
+		self.xlapp.Visible = True
+		win32gui.SetForegroundWindow(self.xlapp.hwnd)
+		self.xlapp.WorkBooks(input_file_name).Activate()
+		self.xlapp.WindowState = win32com.client.constants.xlMaximized
+
 	def change_char_to_num(self, input_text="입력필요"):
 		"""
 		주소를 바꿔주는 것이다
 		문자가 오던 숫자가 오던 숫자로 변경하는 것이다
 		 b를 2로 바꾸어 주는것
 		"""
 		aaa = re.compile("^[a-zA-Z]+$")  # 처음부터 끝가지 알파벳일때
@@ -162,14 +224,47 @@
 				no = no + 1
 		elif result_num != []:
 			result = int(input_text)
 		else:
 			result = "error"
 		return result
 
+	def change_data_position_for_list2d_by_2_index(self, input_list2d, input_no_list):
+		"""
+		2차원 리스트의 자료에서 각 라인별 2개의 위치를 바꾼는것
+		change_position_for_list2d_by_2_index([[1,2,3], [4,5,6]], [0,2])
+		[[1,2,3], [4,5,6]] ==> [[3,2,1], [6,5,4]]
+		"""
+		for before, after in input_no_list:
+			for no in range(len(input_list2d)):
+				value1 = input_list2d[no][before]
+				value2 = input_list2d[no][after]
+				input_list2d[no][before] = value2
+				input_list2d[no][after] = value1
+		return input_list2d
+
+	def change_first_char(self, sheet_name = "", xyxy="", input_2d_list=[]):
+		#엑셀값중, 맨앞의 글자만 변경하는 것
+		#사용법 : change_first_char("", [1,1,100,1], [["'", ""], ["*", ""], [" ", ""],])
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+
+		to_be_changed = []
+		for one in input_2d_list:
+			to_be_changed.append(one[0])
+
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				cell_value = sheet_object.Cells(x, y).Value
+				one_char = str(cell_value[0])
+				if cell_value[0] in to_be_changed:
+					for list_1d in input_2d_list:
+						one_char = one_char.replace(list_1d[0], list_1d[1])
+				sheet_object.Cells(x, y).Value = one_char + cell_value[1:]
+
 	def change_inputcolor_to_rgb(self, input_color):
 		"""
 		입력된 색깔을 rgb로 바꾸는 것
 		"""
 		input_type = type(input_color)
 		if input_type == type(123):
 			result = self.color.change_rgbint_to_rgb(input_color)
@@ -190,14 +285,34 @@
 				result = input_data
 			else:
 				result = [input_data]
 		elif type(input_data) == type("123") or type(input_data) == type(123):
 			result = [[input_data]]
 		return result
 
+	def change_last_char(self, sheet_name = "", xyxy="", input_2d_list=[]):
+		#엑셀값중, 맨앞의 글자만 변경하는 것
+		#사용법 : change_first_char("", [1,1,100,1], [["'", ""], ["*", ""], [" ", ""],])
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+
+		to_be_changed = []
+		for one in input_2d_list:
+			to_be_changed.append(one[0])
+
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				cell_value = sheet_object.Cells(x, y).Value
+				one_char = str(cell_value[-1])
+				if cell_value[-1] in to_be_changed:
+					for list_1d in input_2d_list:
+						one_char = one_char.replace(list_1d[0], list_1d[1])
+				sheet_object.Cells(x, y).Value = cell_value[:-1] + one_char
+
+
 	def change_list1d_to_list2d(self, input_list1d):
 		"""
 		1차원의 리스트를  2차원으로 만드는 것
 		입력 : [1,2,3,4]
 		출력 : [[1], [2], [3], [4],]
 		"""
 		result = []
@@ -230,28 +345,14 @@
 			if max_num == one_len:
 				result.append(one)
 			else:
 				one.extend([input_text] * (max_num - one_len))
 				result.append(one)
 		return result
 
-	def change_data_position_for_list2d_by_2_index(self, input_list2d, input_no_list):
-		"""
-		2차원 리스트의 자료에서 각 라인별 2개의 위치를 바꾼는것
-		change_position_for_list2d_by_2_index([[1,2,3], [4,5,6]], [0,2])
-		[[1,2,3], [4,5,6]] ==> [[3,2,1], [6,5,4]]
-		"""
-		for before, after in input_no_list:
-			for no in range(len(input_list2d)):
-				value1 = input_list2d[no][before]
-				value2 = input_list2d[no][after]
-				input_list2d[no][before] = value2
-				input_list2d[no][after] = value1
-		return input_list2d
-
 	def change_num_to_char(self, input_data="입력필요"):
 		"""
 		입력값 : 27 => 출력값 : aa
 		숫자를 문자로 바꿔주는 것
 		"""
 		re_com = re.compile(r"([0-9]+)")
 		result_num = re_com.match(str(input_data))
@@ -346,19 +447,19 @@
 			# "a2b3"일때
 			result = [temp[0][0], temp[1][0], temp[2][0], temp[3][0]]
 		elif len(temp) == 4 and temp[0][1] != temp[1][1] and temp[0][1] == "string":
 			# "2a3c"일때
 			result = [temp[1][0], temp[0][0], temp[3][0], temp[2][0]]
 		return result
 
-	def change_string_to_address(self, input_text="입력필요"):
+	def change_string_address_to_xyxy(self, input_text="입력필요"):
 		result = self.change_string_address(input_text)
 		return result
 
-	def change_string_address_to_xyxy(self, input_text="입력필요"):
+	def change_string_to_address(self, input_text="입력필요"):
 		result = self.change_string_address(input_text)
 		return result
 
 	def change_value_in_range_as_lower(self, sheet_name="", xyxy=""):
 		"""
 		선택영역안의 모든글자를 소문자로 만들어 주는것
 		screen update를 off로 사용
@@ -674,14 +775,38 @@
 		for x in range(len(datal)):
 			for y in range(len(datal[0])):
 				if datal[x][y] == data2[x][y]:
 					pass
 				else:
 					self.paint_cell_by_excel_colorno(input_sa2[0], [x + start_x, y + start_y], 3)
 
+	def check_differ_at_same_area(self, input_sa1, input_sa2):
+		"""
+		동일한 사이즈의 다른 영역에서 다른 것만 색칠하기
+		"""
+		datal = self.read_value_in_range(input_sa1[0], input_sa1[1])
+		data2 = self.read_value_in_range(input_sa2[0], input_sa2[1])
+		start_x = input_sa2[1][0]
+		start_y = input_sa2[1][1]
+		for x in range(len(datal)):
+			for y in range(len(datal[0])):
+				if datal[x][y] == data2[x][y]:
+					pass
+				else:
+					self.paint_cell_by_excel_colorno(input_sa2[0], [x + start_x, y + start_y], 3)
+
+	def check_filepath(self, file_name):
+		"""
+		경로를 구분하는 \\과 /의 혼돈 삽입으로 다시 확인하고자 한다 가능하면 /를 사용하기를 권장 한다
+		"""
+		file_name = file_name.replace("\\\\","/")
+		file_name = file_name.replace("\\", "/")
+		return file_name
+
+
 	def check_inputcolor_rgb(self, input_color):
 		"""
 		입력값 : 색깔이름
 		출력값 : rgb값
 		"""
 		result = self.change_inputcolor_to_rgb(input_color)
 		return result
@@ -773,14 +898,38 @@
 			address_type = "num"
 			address_int = int(input_text)
 		else:
 			address_int = "error"
 			address_type = "error"
 		return [address_int, address_type, input_text]
 
+	def check_same_data(self, input_list, check_line = 10):
+		"""
+		엑셀의 선택한 자료에서 여러줄을 기준으로 같은 자료만 갖고오기
+		"""
+		result = []
+		base_value = ""
+		xy = self.read_address_in_activecell()
+		for no in input_list:
+			base_value = base_value + str(self.read_cell_value("", [xy[0], no]))
+
+		# 혹시 1보다 작은 숫자가 나올 수있으므로, 최소시작점을 1로하기위해
+		start_x = max(int(xy[0]) - check_line, 1)
+
+		# 위로10개 아래로 10개의 자료를 확인한다
+		for no in range(start_x, start_x+20):
+			cell_value=""
+			for one in input_list:
+				cell_value = cell_value + str(self.read_cell_value("", [no, one]))
+			if base_value == cell_value:
+				# 보통 50개이상의 줄을 사용하지 않으므로 50개를 갖고온다
+				temp = self.read_value_in_range("", [no, 1, no, 50])
+				result.append(temp[0])
+		return result
+
 	def check_sheet_name(self, sheet_name=""):
 		"""
 		시트이름으로 객체를 만들어서 돌려주는 것이다
 		이름이 없으면 현재 활성화된 시트를 객체로 만들어 사용한다
 		"""
 		if sheet_name == "" or sheet_name == None or str(sheet_name).lower() == "activesheet":
 			sheet_object = self.xlapp.ActiveSheet
@@ -888,21 +1037,50 @@
 	def close(self):
 		"""
 		열려진 화일을 닫는것
 		"""
 		self.xlbook.Close(SaveChanges=0)
 		del self.xlapp
 
+	def close_activeworkbook(self):
+		"""
+		열려진 화일을 닫는것
+		"""
+		self.xlbook.Close(SaveChanges=0)
+
+	def close_excel(self):
+		"""
+		열려진 화일을 닫는것
+		"""
+		self.xlbook.Close(SaveChanges=0)
+		del self.xlapp
+
 	def close_workbook(self):
 		"""
 		현재는 close를 시키면 엑셀워크북만이 아니라 엑셀자체도 종료 시킵니다
 		"""
 		self.xlbook.Close(SaveChanges=0)
 		del self.xlapp
 
+	def concate_xlne(self, input_list2d, xy):
+		"""
+		# 선택한 영역의 세로자료들을 다 더해서 제일위의 셀에 다시 넣는것
+		"""
+		x_len = len(input_list2d)
+		y_len = len(input_list2d[0])
+		for y in range(y_len):
+			temp = ""
+			for x in range(x_len):
+				self.write_value_in_cell("", [x + xy[0], y + xy[1]], "")
+				if input_list2d[x][y]:
+					#print(input_list2d[x][y])
+					temp = temp + " " + input_list2d[x][y]
+			#print(temp)
+			self.write_value_in_cell("", [xy[0], y + xy[1]], str(temp).strip())
+
 	def copy_range(self, sheet_name="", xyxy=""):
 		"""
 		영역의 복사까지만 하는 기능이다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		self.check_address_value(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
@@ -953,14 +1131,19 @@
 		self.insert_yyline_in_range(sheet_name, 1)
 		self.insert_yyline_in_range(sheet_name, 1)
 		dic_list = list(py_dic.keys())
 		for no in range(len(dic_list)):
 			sheet_object.Cells(no + 1, 1).Value = dic_list[no]
 			sheet_object.Cells(no + 1, 2).Value = py_dic[dic_list[no]]
 
+	def count_shape_in_sheet(self, sheet_name):
+		sheet_object = self.check_sheet_name(sheet_name)
+		result = sheet_object.Shapes.Count
+		return result
+
 	def count_sheet_nos(self):
 		"""
 		시트의 갯수를 돌려준다
 		"""
 		return self.xlbook.Worksheets.Count
 
 	def count_worksheet_all(self):
@@ -970,85 +1153,85 @@
 		result = self.read_worksheet_numbers()
 		return result
 
 	def data_dic_colorindex_to_colorname(self, input_colorindex):
 		"""
 		색이름으로 엑셀 색번호를 돌려주는것
 		"""
-		dic_colorname_colorindex = self.data_set_basic.vars["excel_colorindex_vs_color_name"]
+		dic_colorname_colorindex = self.var["excel_colorindex_vs_color_name"]
 
 		result = dic_colorname_colorindex[int(input_colorindex)]
 		return result
 
 	def data_dic_colorindex_to_rgbint(self, input_rgbint):
 		"""
 		rgb int값으로 엑셀의 색번호를 돌려주는것
 		"""
-		dic_colorindex_rgbint = self.data_set_basic.vars["excel_colorindex_vs_rgbint"]
+		dic_colorindex_rgbint = self.var["excel_colorindex_vs_rgbint"]
 		result = dic_colorindex_rgbint[int(input_rgbint)]
 		return result
 
 	def data_dic_colorindex_to_rgblist(self, rgblist):
 		"""
 		rgb값으로 엑셀의 색번호를 돌려주는것
 		"""
-		basic = self.data_set_basic.vars["excel_rgblist_vs_colorindex"]
+		basic = self.var["dic_rgb값_vs_엑셀_색번호"]
 		result = basic[rgblist]
 		return result
 
 	def data_dic_colorname_to_colorindex(self, input_colorindex):
 		"""
 		색번호로 색이름을 돌려주는것
 		"""
-		dic_colorname_colorindex = self.data_set_basic.vars["excel_colorname_vs_colorindex"]
+		dic_colorname_colorindex = self.var["dic_색이름_vs_엑셀_색번호"]
 
 		result = dic_colorname_colorindex[int(input_colorindex)]
 		return result
 
 	def data_dic_line_position(self, input_data=""):
 		"""
 		라인 위치에 대한 자료를 돌려준디
 		"""
-		line_position = self.data_set_basic.vars["excel_line_position"]
+		line_position = self.var["dic_선위치_vs_index번호"]
 
 		if input_data in line_position.keys():
 			result = line_position[input_data]
 		else:
 			result = [9]
 		return result
 
 	def data_dic_line_style(self, input_data=""):
 		"""
 		라인 스타일에 대한 자료를 돌려준디
 		"""
-		line_style_dic = self.data_set_basic.vars["excel_line_style_dic"]
+		line_style_dic = self.var["dic_선형태_vs_번호"]
 
 		if input_data in line_style_dic.keys():
 			result = line_style_dic[input_data]
 		else:
 			result = 1
 		return result
 
 	def data_dic_line_thickness(self, input_data=""):
 		"""
 		라인 두께에 대한 자료를 돌려준디
 		"""
-		line_thickness_dic = self.data_set_basic.vars["excel_line_thickness_dic"]
+		line_thickness_dic = self.var["dic_선굵기_vs_번호"]
 
 		if input_data in line_thickness_dic.keys():
 			result = line_thickness_dic[input_data]
 		else:
 			result = 2
 		return result
 
 	def data_dic_rgblist_to_colorindex(self, input_colorindex):
 		"""
 		엑셀의 색번호로 rgb값을 돌려주는것
 		"""
-		dic_colorindex_rgblist = self.data_set_basic.vars["excel_colorindex_vs_rgb_no"]
+		dic_colorindex_rgblist = self.var["dic_rgb값_vs_엑셀_색번호"]
 
 		result = dic_colorindex_rgblist[int(input_colorindex)]
 		return result
 
 	def delete_all_draw_line_in_range(self, sheet_name="", xyxy=""):
 		"""
 		시트의 모든 라인을 지우는 것
@@ -1122,25 +1305,38 @@
 		"""
 		시트안의 모든 값만을 삭제
 		시트를 그대로 둬야하는 경우에 사용
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.Cells.ClearContents()
 
+	def delete_color(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		my_range.Interior.Pattern = -4142
+		my_range.Interior.TintAndShade = 0
+		my_range.Interior.PatternTintAndShade = 0
+
+
 	def delete_color_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역의 색을 지우는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Interior.Pattern = -4142
 		my_range.Interior.TintAndShade = 0
 		my_range.Interior.PatternTintAndShade = 0
 
+	def set_range_nocolor(self, sheet_name, xyxy):
+		self.delete_color_in_range(sheet_name, xyxy)
+
 	def delete_continious_samevalue_in_range(self, sheet_name="", xyxy=""):
 		"""
 		대상 : 선택한 영역
 		밑으로 같은 값들이 있으면 지우는것
 		"""
 
 		sheet_object = self.check_sheet_name(sheet_name)
@@ -1158,33 +1354,55 @@
 		no_list.sort()
 		no_list.reverse()
 		for one in no_list:
 			for x in range(len(input_list2d)):
 				del input_list2d[x][one]
 		return input_list2d
 
+	def delete_linecolor(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.Interior.Pattern = 0
+		my_range.Interior.PatternTintAndShade = 0
+
+
 	def delete_linecolor_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 라인의 색을 지우는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Interior.Pattern = 0
 		my_range.Interior.PatternTintAndShade = 0
 
+	def delete_link(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.Hyperlinks.Delete()
+
+
 	def delete_link_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 링크를 삭제하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Hyperlinks.Delete()
 
+	def delete_memo(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.ClearComments()
+
+
 	def delete_memo_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 메모를 삭제하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
@@ -1211,14 +1429,18 @@
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 
 				cell_value = sheet_object.Cells(x, y).Value
 				if cell_value != "" or cell_value != None or cell_value != None:
 					sheet_object.Cells(x, y).Value = cell_value[int(num):]
 
+	def delete_rangename(self, range_name):
+		self.xlbook.Names(range_name).Delete()
+
+
 	def delete_rangename_all(self):
 		"""
 		모든 rangename을 삭제하는 것
 		"""
 		aaa = self.xlapp.Names
 		for one in aaa:
 			ddd = str(one.Name)
@@ -1233,14 +1455,22 @@
 		"""
 		result = self.xlbook.Names(range_name).Delete()
 		return result
 
 	def delete_rangname_for_panthom(self):
 		self.delete_panthom_rangname()
 
+	def delete_rangname_panthom(self):
+		aaa = self.xlbook.Names
+		cnt = self.xlbook.Names.Count
+		for num in range(1, cnt + 1):
+			aaa = self.xlbook.Names(num).Name
+			if aaa.find("!") < 0:
+				self.xlbook.Names(aaa).Delete()
+
 	def delete_samevalue_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 같은 값을 지우는 것이다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		set_a = set([])
@@ -1255,21 +1485,32 @@
 					len_new = len(set_a)
 					if len_old == len_new:
 						sheet_object.Cells(x, y).Value = ""
 
 	def delete_samevalue_in_range_by_many_column_are_same(self, sheet_name="", xyxy=""):
 		self.delete_xxline_value_in_range_by_same_line(sheet_name, xyxy)
 
+	def delete_shape_all_in_sheet(self, sheet_name):
+		sheet_object = self.check_sheet_name(sheet_name)
+		shape_no = sheet_object.Shapes.Count
+		if shape_no > 0:
+			for aa in range(shape_no, 0, -1):
+				sheet_object.Shapes(aa).Delete()
+
 	def delete_shape_by_name(self, sheet_name="", shape_name="입력필요"):
 		"""
 		객체의 이름으로 제거하는것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.Shapes(shape_name).Delete()
 
+	def delete_shape_in_sheet(self, sheet_name, shape_name):
+		sheet_object = self.check_sheet_name(sheet_name)
+		sheet_object.Shapes(shape_name).Delete()
+
 	def delete_sheet(self, sheet_name=""):
 		self.delete_sheet_by_name(sheet_name)
 
 	def delete_sheet_by_name(self, sheet_name=""):
 		"""
 		시트하나 삭제하기
 		"""
@@ -1494,39 +1735,61 @@
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		for y in range(y1, y2 + 1):
 			if divmod(y-y1+1, step_no)[1] == 0:
 				sheet_object.Range(sheet_object.Cells(x1, y), sheet_object.Cells(x2, y)).ClearContents()
 
+	def delete_yy_line_as_empty(self, sheet_name, yy_list):
+		sheet_object = self.check_sheet_name(sheet_name)
+		for y in range(yy_list[0], yy_list[1]+1):
+			changed_address = str(y) + ":" + str(y)
+			num = self.xlbook.WorksheetFunction.CountA(sheet_object.Range(changed_address))
+			if num == 0:
+				sheet_object.Rows(changed_address).Delete()
+
+
 	def delete_yyline(self, sheet_name="", yy=""):
 		"""
 		선택한영역에서 여러개의 y줄을 삭제한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		y1, y2 = self.check_yy_address(yy)
 		sheet_object.Columns(y1 + ':' + y2).Delete()
 
+
+
 	def delete_yyline_in_sheet(self, sheet_name="", yy=""):
 		self.delete_yyline(sheet_name, yy)
 
+	def draw_bottomline(self, sheet_name, xyxy, line_style, thickness, scolor):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		rgb_list = self.color.change_color_to_rgb(scolor)
+		my_range.Borders(9).Color = self.color.change_rgb_to_rgbint(rgb_list)
+		my_range.Borders(9).Weight = thickness
+		my_range.Borders(9).LineStyle = line_style
+
+
 	def draw_bottomline_in_range(self, sheet_name="", xyxy="", line_style="basic", thickness="basic", color="blu"):
 		"""
 		선택영역에서 선을 긋는것, 맨마지막 라인에 선긋기
 		"""
 		self.draw_line_one_in_range(sheet_name, xyxy, line_style, thickness, color, 9)
 
 	def draw_detail_line_in_range(self, **input):
 		"""
 		선택영역에서 선을 긋는것
 		선긋기를 좀더 상세하게 사용할수 있도록 만든것
 		밐의 base_data의 값들을 이용해서 입력하면 된다
 		"""
-		enum_line = self.data_set_basic.vars["enum_line"]
-		base_data = self.data_set_basic.vars["base_cell_data"]
+		enum_line = self.var["dic_선모양_vs_index번호"]
+		base_data = self.var["base_cell_data"]
 		# 기본자료에 입력받은값을 update하는것이다
 		sheet_object = self.check_sheet_name("")
 		base_data.update(input)
 		sheet = self.check_sheet_name(base_data["sheet_name"])
 		set_line = sheet_object.Shapes.AddLine(base_data["xyxy"][0], base_data["xyxy"][1], base_data["xyxy"][2], base_data["xyxy"][3])
 		set_line.Select()
 		set_line.Line.ForeColor.RGB = base_data["color"]
@@ -1543,22 +1806,81 @@
 		result = set_line.Name
 		return result
 
 	def draw_innerx_line_in_range(self, sheet_name="", xyxy="", line_style="basic", thickness="basic", color="blu"):
 		"""	선택영역에서 선을 긋는것, 안쪽에 x라인 선긋기 """
 		self.draw_line_one_in_range(sheet_name, xyxy, line_style, thickness, color, 12)
 
+	def draw_innerxline(self, sheet_name, xyxy, line_style, thickness, scolor):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		rgb_list = self.color.change_color_to_rgb(scolor)
+		my_range.Borders(12).Color = self.color.change_rgb_to_rgbint(rgb_list)
+		my_range.Borders(12).Weight = thickness
+		my_range.Borders(12).LineStyle = line_style
+
+
 	def draw_innery_line_in_range(self, sheet_name="", xyxy="", line_style="basic", thickness="basic", color="blu"):
 		"""	선택영역에서 선을 긋는것, 안쪽에 y라인 선긋기 """
 		self.draw_line_one_in_range(sheet_name, xyxy, line_style, thickness, color, 11)
 
+	def draw_inneryline(self, sheet_name, xyxy, line_style, thickness, scolor):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		rgb_list = self.color.change_color_to_rgb(scolor)
+		my_range.Borders(11).Color = self.color.change_rgb_to_rgbint(rgb_list)
+		my_range.Borders(11).Weight = thickness
+		my_range.Borders(11).LineStyle = line_style
+
 	def draw_left_line_in_range(self, sheet_name="", xyxy="", line_style="basic", thickness="basic", color="blu"):
 		"""	선택영역에서 선을 긋는것, 왼쪽에 선긋기 """
 		self.draw_line_one_in_range(sheet_name, xyxy, line_style, thickness, color, 7)
 
+	def draw_leftline(self, sheet_name, xyxy, line_style, thickness, scolor):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+
+		rgb_list = self.color.change_color_to_rgb(scolor)
+		my_range.Borders(7).Color = self.color.change_rgb_to_rgbint(rgb_list)
+		my_range.Borders(7).Weight = thickness
+		my_range.Borders(7).LineStyle = line_style
+
+
+	def draw_line(self, sheet_name, xyxy, input_list):
+		"""
+	  draw_range_line(sheet_name="", xyxy="", input_list)
+	  [선의위치, 라인스타일, 굵기, 색깔]
+	  입력예 : [7,1,2,1], ["left","-","t0","bla"]
+	  선의위치 (5-대각선 오른쪽, 6-왼쪽대각선, 7:왼쪽, 8;위쪽, 9:아래쪽,
+			10:오른쪽, 11:안쪽세로, 12:안쪽가로)
+	  라인스타일 (1-실선, 2-점선, 3-가는점선, 6-굵은실선,
+	  굵기 (0-이중, 1-얇게, 2-굵게)
+	  색깔 (0-검정, 1-검정, 3-빨강),
+	  """
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		line_type = self.var["dic_선위치_vs_번호"]
+		line_style_dic = self.var["dic_선형태_vs_번호"]
+		weight_dic = self.var["dic_선굵기_vs_번호"]
+
+		rgb_list = self.color.change_color_to_rgb(input_list[3])
+		my_range.Borders(line_type[input_list[0]]).Color = self.color.change_rgb_to_rgbint(rgb_list)
+		my_range.Borders(line_type[input_list[0]]).Weight = weight_dic[input_list[2]]
+		my_range.Borders(line_type[input_list[0]]).LineStyle = line_style_dic[input_list[1]]
+
+
+
 	def draw_line_in_pxyxy_range(self, sheet_name, line_xyxy, rgb_list):
 		"""
 		선택영역에서 선을 긋는것
 		pixel을 기준으로 선긋기
 		선을 그을때는 위치와 넓이 높이로 긋는데, change_xyxy_to_pxyxy을 사용하면 셀위치를 그렇게 바꾸게 만든다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
@@ -1573,17 +1895,17 @@
 		"""
 		입력예 : [선의위치, 색깔, 라인스타일, 굵기] ==> [7,1,2,1], "", "",""
 		""으로 된것이 기본으로 설정하는 것이다
 		"l": left, "t": top, "b": bottom, "r": right, "h": horizental, "v": vertical, "a": all,"o": outside,"/": "/","\\": "\",
 		""으로 된것이 기본으로 설정하는 것이다
 		color = rgb 값
 		"""
-		line_position = self.data_set_basic.vars["excel_line_position"]
-		line_thickness_dic = self.data_set_basic.vars["excel_line_thickness_dic"]
-		line_style_dic = self.data_set_basic.vars["excel_line_style_dic"]
+		line_position = self.var["dic_선위치_vs_index번호"]
+		line_thickness_dic = self.var["dic_선굵기_vs_번호"]
+		line_style_dic = self.var["dic_선형태_vs_번호"]
 
 
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		#print(scolor)
@@ -1611,14 +1933,36 @@
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		rgb_list = self.color.change_scolor_to_rgb(color)
 		my_range.Borders(line_position).Color = self.color.change_rgb_to_rgbint(rgb_list)
 		my_range.Borders(line_position).Weight = self.data_dic_line_thickness(thickness)
 		my_range.Borders(line_position).LineStyle = self.data_dic_line_style(line_style)
 
+	def draw_rightline(self, sheet_name, xyxy, line_style, thickness, scolor):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		rgb_list = self.color.change_color_to_rgb(scolor)
+		my_range.Borders(10).Color = self.color.change_rgb_to_rgbint(rgb_list)
+		my_range.Borders(10).Weight = thickness
+		my_range.Borders(10).LineStyle = line_style
+
+
+	def draw_topline(self, sheet_name, xyxy, line_style, thickness, scolor):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		rgb_list = self.color.change_color_to_rgb(scolor)
+		my_range.Borders(8).Color = self.color.change_rgb_to_rgbint(rgb_list)
+		my_range.Borders(8).Weight = thickness
+		my_range.Borders(8).LineStyle = line_style
+
+
 	def draw_triangle(self, xyxy, per=100, reverse=1, size=100):
 		"""
 		직각삼각형
 		정삼각형에서 오른쪽이나 왼쪽으로 얼마나 더 간것인지
 		100이나 -100이면 직삼각형이다
 		사각형은 왼쪽위에서 오른쪽 아래로 만들어 진다
 		"""
@@ -1823,14 +2167,62 @@
 		xx영역을 객체로 돌려주는것
 		"""
 		new_x = self.check_xx_address(xx)
 		sheet_object = self.check_sheet_name(sheet_name)
 		result = sheet_object.Rows(str(new_x[0]) + ':' + str(new_x[1]))
 		return result
 
+	def get_xy_list_for_circle(self, r, precious=10, xy=[0, 0]):
+		"""
+		엑셀을 기준으로, 반지름이 글자를 원으로 계속 이동시키는 것
+		r : 반지름
+		precious : 얼마나 정밀하게 할것인지, 1도를 몇번으로 나누어서 계산할것인지
+		"""
+		result = []
+		temp = []
+		for do_1 in range(1, 5):
+			for do_step in range(90 * precious + 1):
+				degree = (do_1 * do_step) / precious
+				# r을 더하는 이유는 마이너스는 않되므로 x, y측을 이동시키는것
+				x = math.cos(degree) * r
+				y = math.sin(degree) * r
+				new_xy = [int(round(x)), int(round(y))]
+
+				if not new_xy in temp:
+					temp.append(new_xy)
+		area_1 = []
+		area_2 = []
+		area_3 = []
+		area_4 = []
+
+		for x, y in temp:
+			new_x = x + r + 1 + xy[0]
+			new_y = y + r + 1 + xy[1]
+
+			if x >= 0 and y >= 0:
+				area_1.append([new_x, new_y])
+			elif x >= 0 and y < 0:
+				area_2.append([new_x, new_y])
+			elif x < 0 and y < 0:
+				area_3.append([new_x, new_y])
+			elif x < 0 and y >= 0:
+				area_4.append([new_x, new_y])
+		area_1.sort()
+		area_1.reverse()
+		area_2.sort()
+		area_3.sort()
+		area_4.sort()
+		area_4.reverse()
+
+		result.extend(area_2)
+		result.extend(area_1)
+		result.extend(area_4)
+		result.extend(area_3)
+		return result
+
 	def get_yyline_object(self, sheet_name, yy):
 		"""
 		yy영역을 객체로 돌려주는것
 		"""
 		new_y = self.check_yy_address(yy)
 		sheet_object = self.check_sheet_name(sheet_name)
 		result = sheet_object.Columns(str(new_y[0]) + ':' + str(new_y[1]))
@@ -1858,14 +2250,23 @@
 	def input_messagebox_value(self, text_01="halmoney"):
 		"""
 		입력창을 만들어서 입력값을 받는것
 		"""
 		result = self.xlapp.InputBox(text_01)
 		return result
 
+	def insert_excel_function_in_cell(self, sheet_name, xy, input_fucntion, input_xyxy):
+		result = ""
+		sheet_object = self.check_sheet_name(sheet_name)
+		range = self.change_xyxy_to_r1r1(input_xyxy)
+		x1, y1, x2, y2 = self.check_address_value(xy)
+		result = "="+input_fucntion+"("+range+")"
+
+		sheet_object.Cells(x1, y1).Value = result
+
 	def insert_image_in_sheet(self, sheet_name, file_path, xywh, link=0, image_in_file=1):
 		self.insert_picture_in_sheet(self, sheet_name, file_path, xywh, link, image_in_file)
 
 	def insert_image_in_xyxy(self, sheet_name, xyxy, file_path):
 		"""
 		image화일을 넣는것
 		선택한 영역안에 자동으로 올수있도록 만들어 보자
@@ -1935,35 +2336,28 @@
 			mok, namuji = divmod(x, int(step_no))
 			if namuji == step_no - 1:
 				#print("===>", x + x1)
 				x_no = self.change_char_to_num(x + x1)
 				#print("===>", x_no)
 				sheet_object.Range(str(x_no) + ':' + str(x_no)).Insert(-4121)
 
-	def insert_excel_function_in_cell(self, sheet_name, xy, input_fucntion, input_xyxy):
-		result = ""
-		sheet_object = self.check_sheet_name(sheet_name)
-		range = self.change_xyxy_to_r1r1(input_xyxy)
-		x1, y1, x2, y2 = self.check_address_value(xy)
-		result = "="+input_fucntion+"("+range+")"
-
-		sheet_object.Cells(x1, y1).Value = result
-
 	def insert_xxline(self, sheet_name, xx_list):
 		"""
 		가로열을 한줄삽입하기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1 = self.change_char_to_num(xx_list[0])
 		x2 = self.change_char_to_num(xx_list[1])
 		min_x1 = min(x1, x2)
 		max_x2 = max(x1, x2)
 		for num in range(max_x2+1, min_x1, -1):
 			sheet_object.Range(str(num) + ':' + str(num)).Insert(-4121)
 
+
+
 	def insert_xxline_in_range(self, sheet_name="", xx_list="입력필요"):
 		"""
 		가로열을 한줄삽입하기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		if type(xx_list) == type([]) and len(xx_list) == 1:
 			x2 = x1 = self.change_char_to_num(xx_list[0])
@@ -2052,14 +2446,20 @@
 		new_range_y.sort()
 		if x11 <= new_range_x[1] and x12 >= new_range_x[2] and y11 <= new_range_y[1] and y12 >= new_range_y[1]:
 			result = [new_range_x[1], new_range_y[1], new_range_x[2], new_range_y[2]]
 		else:
 			result = "교차점없음"
 		return result
 
+	def is_empty(self, x_no):
+		x1 = self.change_char_to_num(x_no)
+		result = self.xlbook.WorksheetFunction.CountA(vars["sheet"].Columns(x1).EntireColumn)
+		return result
+
+
 	def is_empty_xline(self, sheet_name, no):
 		"""
 		열전체가 빈 것인지 확인해서 돌려준다
 		현재의 기능은 한줄만 가능하도록 하였다
 		다음엔 영역이 가능하도록 하여야 겠다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
@@ -2072,18 +2472,70 @@
 		현재의 기능은 한줄만 가능하도록 하였다
 		다음엔 영역이 가능하도록 하여야 겠다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		result = self.xlapp.WorksheetFunction.CountA(sheet_object.Columns(no).EntireColumn)
 		return result
 
+	def lock_off(self, sheet_name, password="1234"):
+		sheet_object = self.check_sheet_name(sheet_name)
+
+		sheet_object.Unprotect(password)
+
+
+	def lock_on(self, sheet_name, password="1234"):
+		sheet_object = self.check_sheet_name(sheet_name)
+
+		sheet_object.protect(password)
+
 	def lock_sheet(self, sheet_name="", password="1234"):
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.protect(password)
 
+	def lock_with_password(self, pwd="1234567890"):
+		repeat_no = 4
+		count = 0
+		for a in itertools.product(pwd, repeat=repeat_no):
+			count += 1
+			temp_pwd = ("".join(map(str, a)))
+			try:
+				#pcell_dot.setup.lock_off(vars["sheet_name"], temp_pwd)
+				pass
+			except:
+				pass
+			else:
+				break
+		pass
+
+	def make_password(self, isnum="yes", istext_small="yes", istext_big="yes", isspecial="no", len_num=10):
+		"""
+		엑셀시트의 암호를 풀기위해 암호를 계속 만들어서 확인하는 것
+		"""
+		check_char = []
+		if isnum == "yes":
+			check_char.extend(list(string.digits))
+		if istext_small == "yes":
+			check_char.extend(list(string.ascii_lowercase))
+		if istext_big == "yes":
+			check_char.extend(list(string.ascii_uppercase))
+		if isspecial == "yes":
+			for one in "!@#$%^*_-":
+				check_char.extend(one)
+
+		zz = combinations_with_replacement(check_char, len_num)
+		for aa in zz:
+			try:
+				pswd = "".join(aa)
+				#print(pswd)
+				self.unlock_sheet("", pswd)
+				break
+				#print("발견", pswd)
+			except:
+				pass
+
 	def make_vba_module(self, vba_code, macro_name):
 		"""
 		텍스트로 만든 매크로 코드를 실행하는 코드이다
 		"""
 		new_vba_code = "Sub " + macro_name + "()" + vba_code + "End Sub"
 		mod = self.xlbook.VBProject.VBComponents.Add(1)
 		mod.CodeModule.AddFromString(new_vba_code)
@@ -2219,14 +2671,49 @@
 				if before < after:
 					after = after -1
 				value = input_list2d[no][before]
 				del input_list2d[no][before]
 				input_list2d[no].insert(int(after), value)
 		return input_list2d
 
+	def move_shape(self, sheet_name, shape_obj, top, left):
+		# shape_obj : 이동시림 도형 이름
+		sheet_object = self.check_sheet_name(sheet_name)
+		oShape = sheet_object.Shapes(shape_obj)
+		oShape.Top = oShape.Top + top
+		oShape.Left = oShape.left + left
+
+	def move_to_bottom(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.End(- 4121).Select()
+
+
+	def move_to_leftend(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.End(- 4159).Select()
+
+
+	def move_to_rightend(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.End(- 4161).Select()
+
+
+	def move_to_top(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.End(- 4162).Select()
+
+
 	def move_value_in_range_to_left_except_emptycell(self, sheet_name="", xyxy=""):
 		"""
 		x열을 기준으로 값이 없는것은 왼쪽으로 옮기기
 		전체영역의 값을 읽어오고, 하나씩 다시 쓴다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
@@ -2301,23 +2788,46 @@
 		y1, y2 = self.check_yy_address(yy_list[0])
 		sheet_object_1.Columns(y1 + ':' + y2).Cut()
 
 		sheet_object_2 = self.check_sheet_name(sheet_name_list[1])
 		y1_new, y2_new = self.check_yy_address(yy_list[1])
 		sheet_object_2.Columns(y1_new + ':' + y2_new).Insert()
 
+	def open_file(self, filename=""):
+		"""
+		"""
+		self.path_full = self.check_filepath(filename)
+		self.file_name_only = self.path_full.split("/")[-1]
+		if filename.lower() == 'new'or filename == "":
+			#빈것으로 된 경우는 새로운 workbook < 연다는 뜻으로 해석
+			try:
+				self.xlapp.Windowstate = -4137
+				self.xlbook = self.xlapp.WorkBooks.Add()
+			except:
+				win32gui.MessageBox(0, "There is no Activeworkbook", "www.halmoney.com", 0)
+		else:
+				#	열린 화일중에 같은것이 있는지 확인하는 것
+				file_name_list = self.read_opened_workbook_filename_all()
+				if self.file_name_only in file_name_list:
+					pass
+				else:
+					try:
+						self.xlbook = self.xlapp.Workbooks.Open(self.path_full)
+					except:
+						win32gui.MessageBox(0, "화일이름이나 경로를 다시한번 확인해 보시기 바랍니다”, .halmoney.com", 0)
+
 	def paint_cell_by_excel_colorno(self, sheet_name, xy, excel_color_no="입력필요"):
 		"""
 		paint_color(sheet_name, xyxy, input_data="입력필요")
 		선택 셀에 색깔을 넣는다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		self.check_address_value(xy)
 
-		rgbvalue = self.data_set_basic.vars["rgb_56_for_excel"][excel_color_no]
+		rgbvalue = self.var["rgb_56_for_excel"][excel_color_no]
 
 		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
 		sheet_object.Cells(xy[0], xy[1]).Interior.Color = int(rgb_to_int)
 
 	def paint_cell_by_rgb(self, sheet_name, xy, input_color="입력필요"):
 		"""
 		paint_color(sheet_name, xyxy, input_data="입력필요")
@@ -2387,14 +2897,23 @@
 				temp_int = 0
 				for one_word in basic_list:
 					if re.match('(.*)' + one_word + '(.*)', str(cell_value)):
 						temp_int = temp_int + 1
 				if temp_int == total_no:
 					self.paint_color_in_range(sheet_name, [x, y], "yel")
 
+	def paint_color_name_in_cell(self, sheet_name, xyxy, input_color):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		input_data = self.color.check_input_color(input_color)
+		rgb_to_int = (int(input_data[2])) * (256 ** 2) + (int(input_data[1])) * 256 + int(input_data[0])
+		my_range.Interior.Color = rgb_to_int
+
 	def paint_font_in_cell_by_rgb(self, sheet_name="", xyxy="", rgb=""):
 		"""
 		셀안의 폰트 색깔을 넣는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
@@ -2408,14 +2927,24 @@
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		input_data = self.color.change_scolor_to_rgb(font_color)
 		rgb_to_int = (int(input_data[2])) * (256 ** 2) + (int(input_data[1])) * 256 + int(input_data[0])
 		my_range.Font.Color = rgb_to_int
 
+	def paint_fontcolor(self, sheet_name, xyxy, input_color):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		rgbvalue = self.color.change_color_to_rgb(input_color)
+		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
+		my_range.Interior.Color = rgb_to_int
+
+
 	def paint_maxvalue_in_range_in_each_xline(self, sheet_name="", xyxy=""):
 		"""
 		각 x라인별로 최대값에 색칠하는 것
 		"""
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		all_data = self.read_value_in_range(sheet_name, [x1, y1, x2, y2])
@@ -2503,14 +3032,24 @@
 				else:
 					len_old = len(set_a)
 					set_a.add(value)
 					len_new = len(set_a)
 					if len_old == len_new:
 						self.paint_cell_by_excel_colorno(sheet_name, [x, y], excelcolorno)
 
+	def paint_rgb_in_cell(self, sheet_name, xyxy, input_rgb):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		# RGB값을 색칠하는 방법
+		rgb_to_int = (int(input_rgb[2])) * (256 ** 2) + (int(input_rgb[1])) * 256 + int(input_rgb[0])
+		my_range.Interior.Color = rgb_to_int
+
+
 	def paint_samevalue_in_range_by_scolor(self, sheet_name="", xyxy="", input_color="gray"):
 		"""
 		선택한 영역에서 2번이상 반복된것만 색칠하기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
@@ -2523,23 +3062,48 @@
 				else:
 					len_old = len(set_a)
 					set_a.add(value)
 					len_new = len(set_a)
 					if len_old == len_new:
 						self.paint_cell_by_scolor(sheet_name, [x, y], input_color)
 
+	def paint_scolor_in_cell(self, sheet_name, xyxy, input_color):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		rgbvalue = self.color.change_color_to_rgb(input_color)
+		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
+		my_range.Interior.Color = rgb_to_int
+
+
 	def paint_sheet_tab_by_scolor(self, sheet_name, input_color="입력필요"):
 		"""
 		시트탭의 색을 넣는것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		rgbvalue = self.color.change_scolor_to_rgb(input_color)
 		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
 		sheet_object.Tab.Color = rgb_to_int
 
+	def paint_spacecell(self, sheet_name="", xyxy="", input_color="red"):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+
+		for x in range(x1, x2+1):
+			for y in range(y1, y2+1):
+				cell_value = sheet_object.Cells(y, x).Value
+				com = re.compile("^\s+")
+				if cell_value != None:
+					if com.search(cell_value):
+						input_data = self.color.check_input_color(input_color)
+						rgb_to_int = (int(input_data[2])) * (256 ** 2) + (int(input_data[1])) * 256 + int(
+							input_data[0])
+						sheet_object.Cells(y, x).Interior.Color = rgb_to_int
+
 	def paint_spacecell_in_range_by_scolor(self, sheet_name="", xyxy="", input_color="입력필요"):
 		"""
 		빈셀처럼 보이는데 space문자가 들어가 있는것 찾기
 		선택한 영역의 셀을 하나씩 읽어와서 re모듈을 이용해서 공백만 있는지 확인한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
@@ -2559,14 +3123,25 @@
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		rgbvalue = self.color.change_scolor_to_rgb(input_color)
 		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
 		my_range.Font.Color = rgb_to_int
 
+	def paint_textcolor(self, sheet_name, xyxy, input_color):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		rgbvalue = self.color.change_color_to_rgb(input_color)
+		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
+
+		my_range.Font.Color = rgb_to_int
+
+
 	def paste_range(self, sheet_name="", xyxy=""):
 		"""
 		영역에 붙여넣기 하는것
 		"""
 
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
@@ -2751,14 +3326,24 @@
 				result["line_x2_dic"]["style"] = one_cell.Borders(12).LineStyle
 				result["line_x2_dic"]["color"] = one_cell.Borders(12).Color
 				result["line_x2_dic"]["colorindex"] = one_cell.Borders(12).ColorIndex
 				result["line_x2_dic"]["thick"] = one_cell.Borders(12).Weight
 				result["line_x2_dic"]["tintandshade"] = one_cell.Borders(12).TintAndShade
 		return result
 
+	def read_all_shape_names(self, sheet_name=""):
+		sheet_object = self.check_sheet_name(sheet_name)
+		drawings_nos = sheet_object.Shapes.count
+		result = []
+		if drawings_nos > 0:
+			for num in range(sheet_object.Shapes.count, 0, -1):
+				# Range를 앞에서부터하니 삭제하자마자 번호가 다시 매겨져서, 뒤에서부터 삭제하니 잘된다
+				result.append(sheet_object.Shapes(num).Name)
+		return result
+
 	def read_cell_value(self, sheet_name="", xyxy=""):
 		#보관용
 		result = self.read_value_in_cell(sheet_name, xyxy)
 		return result
 
 	def read_color_in_cell(self, sheet_name="", xyxy=""):
 		"""
@@ -2806,14 +3391,17 @@
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Cells(x1, y1)
 		result = my_range.Font.Color
 		return result
 
+	def read_fullname_for_workbook(self):
+		return self.xlapp.FullName
+
 	def read_general_value(self):
 		"""
 		몇가지 엑셀에서 자주사용하는 것들정의
 		엑셀의 사용자, 현재의 경로, 화일이름, 현재시트의 이름
 		"""
 		result = []
 		result.append(self.xlapp.ActiveWorkbook.Name)
@@ -2846,14 +3434,31 @@
 	def read_opened_workbook_filename_all(self):
 		# 모든 열려있는 엑셀화일의 이름을 갖고옵니다
 		result = []
 		for one in self.xlapp.Workbooks:
 			result.append(one.Name)
 		return result
 
+	def read_path_for_workbook(self):
+		return self.xlapp.Path
+
+
+
+
+	def read_pixel_size_in_cell(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		rng_x_coord = my_range.Left
+		rng_y_coord =my_range.Top
+		rng_width = my_range.Width
+		rng_height = my_range.Height
+		return [rng_x_coord, rng_y_coord, rng_width, rng_height]
+
 	def read_range_value(self, sheet_name="", xyxy=""):
 		#보관용
 		result = self.read_value_in_range(sheet_name, xyxy)
 		return result
 
 	def read_rangename_all(self):
 		"""
@@ -2902,14 +3507,19 @@
 				result[2] = (string.ascii_lowercase.index(result[2]) + 1)
 			else:
 				aaa = (string.ascii_lowercase.index(result[2][0]) + 1) * 26
 				result[2] = aaa + (string.ascii_lowercase.index(result[2][1]) + 1)
 		final_data = [int(result[1]), int(result[0]), int(result[3]), int(result[2])]  # 2005-02-17 추가
 		return final_data
 
+	def read_shape_name_by_shape_no(self, sheet_name,shape_no=""):
+		sheet_object = self.check_sheet_name(sheet_name)
+		result = sheet_object.Shapes(shape_no).Name
+		return result
+
 	def read_shape_name_in_sheet_by_no(self, sheet_name="", shape_no="입력필요"):
 		"""
 		번호로 객체의 이름을 갖고오는것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		result = sheet_object.Shapes(shape_no).Name
 		return result
@@ -3128,14 +3738,21 @@
 			if len(x_list) < resize[1] or resize[1] == 0:
 				pass
 			else:
 				x_list = xy_list[:resize[0]]
 			result.append(x_list)
 		return result
 
+	def rotate_shape(self, sheet_name, shape_obj, degree):
+		# 도형을 회전시키는 것
+		# shape _ obi :이동시킬 도형 이름
+		sheet_object = self.check_sheet_name(sheet_name)
+		oShape = sheet_object.Shapes(shape_obj)
+		oShape.IncrementRotation(degree)
+
 	def run_vba_module(self, vba_code, macro_name):
 		"""
 		텍스트로 만든 매크로 코드를 실행하는 코드이다
 		"""
 		new_vba_code = "Sub " + macro_name + "()//n" + vba_code + "End Sub"
 		mod = self.xlbook.VBProject.VBComponents.Add(1)
 		mod.CodeModule.AddFromString(new_vba_code)
@@ -3176,14 +3793,15 @@
 		영역을 선택한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Select()
 
+
 	def select_sheet(self, sheet_name=""):
 		"""
 		현재의 엑셀중에서 활성화된 시트의 이름을 돌려준다
 		"""
 		if sheet_name == None or sheet_name == "":
 			self.show_messagebox_with_value("시트이름을 다시한번 확인 해 주십시요")
 		elif sheet_name in self.read_sheet_name_all():
@@ -3191,14 +3809,20 @@
 
 	def select_top_line_in_range(self, sheet_name="", xyxy=""):
 		""" 영역의 제일 위로 이동 """
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		sheet_object.Cells(x1, y1).Select()
 
+	def set_autofilter(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.Columns.AutoFilter(1)
+
 	def set_autofit_in_range(self, sheet_name="", xyxy="all"):
 		""" 자동 맞춤을 실시 """
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		new_y1 = self.change_num_to_char(y1)
 		new_y2 = self.change_num_to_char(y2)
 		if xyxy == "" or xyxy == "all":
@@ -3211,17 +3835,36 @@
 		영역안의 글씨체를 진하게 만든다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Font.Bold = True
 
+	def set_capital_in_range(self):
+		for x in range(vars["x1"], vars["x2"] + 1):
+			for y in range(vars["y1"], vars["y2"] + 1):
+				one_value = vars["sheet"].Cells(y, x).Value
+				if one_value == None:
+					one_value = ""
+				vars["sheet"].Cells(y, x).Value = str(one_value.capitalize())
+
 	def set_cell_color(self, sheet_name, xy, input_color="입력필요"):
 		self.paint_cell_by_scolor(sheet_name, xy, input_color)
 
+	def set_color_bar_by_no(self, sheet_name, xyxy, color_value=255):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		my_range.FormatConditions.AddDatabar
+		my_range.FormatConditions(1).NegativeBarFormat.ColorType = 0  # xlDataBarColor =0
+		my_range.FormatConditions(1).NegativeBarFormat.Color.Color = color_value
+		my_range.FormatConditions(1).NegativeBarFormat.Color.TintAndShade = 0
+
+
 	def set_conditional_in_range(self):
 		""" 조건부서식을 좀더 사용하기 쉽도록 변경이 필요 """
 		sheet_object = self.check_sheet_name("")
 		my_range = sheet_object.Range(sheet_object.Cells(1, 1), sheet_object.Cells(20, 20))
 		formula1 = ' = IF($A1 = "", TRUE, FALSE)'
 		# win32com.client.constants.xlCellValue = > 1
 		# win32com.client.constants.xlGreaterEqual = > 7
@@ -3232,23 +3875,14 @@
 		my_range.FormatConditions(1).Font.TintAndShade = 0
 		my_range.FormatConditions(1).Interior.PatternColorIndex = 1
 		my_range.FormatConditions(1).Interior.Color = 5296274
 		my_range.FormatConditions(1).Interior.TintAndShade = 0
 		my_range.FormatConditions(1).StopIfTrue = False
 
 
-	def check_filepath(self, file_name):
-		"""
-		경로를 구분하는 \\과 /의 혼돈 삽입으로 다시 확인하고자 한다 가능하면 /를 사용하기를 권장 한다
-		"""
-		file_name = file_name.replace("\\\\","/")
-		file_name = file_name.replace("\\", "/")
-		return file_name
-
-
 	def set_font_in_range(self, sheet_name="", xyxy="", font="입력필요"):
 		"""
 		영역에 글씨체를 설정한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
@@ -3317,31 +3951,69 @@
 	def set_gridline_onoff(self):
 		""" 그리드라인을 껏다 켰다하는 것 """
 		if self.xlapp.ActiveWindow.DisplayGridlines == 0:
 			self.xlapp.ActiveWindow.DisplayGridlines = 1
 		else:
 			self.xlapp.ActiveWindow.DisplayGridlines = 0
 
+	def set_height_in_range(self, sheet_name, xyxy, height=13.5):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.RowHeight = height
+
+
+
 	def set_height_in_xxline(self, sheet_name, xx, height=13.5):
 		"""
 		가로줄의 높이를 설정
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		my_range = sheet_object.Range(sheet_object.Cells(xx[0], 1), sheet_object.Cells(xx[1], 1))
 		my_range.RowHeight = height
 
+	def set_lower_in_range(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				value = sheet_object.Cells(y, x).Value
+				sheet_object.Cells(y, x).Value = str(value.lower())
+
+	def set_ltrim_in_range(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				value = sheet_object.Cells(y, x).Value
+				sheet_object.Cells(y, x).Value = str(value.lstrip())
+
+
 	def set_merge_in_range(self, sheet_name="", xyxy=""):
 		"""
 		셀들을 병합하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Merge(0)
 
+	def set_name_in_range(self, name):
+		self.xlbook.Names.Add(name, vars["range"])
+
+
+	def set_numberformat(self, sheet_name, xyxy, numberformat):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		my_range.NumberFormat = numberformat
+
+
+
 	def set_numberformat_in_cell(self, sheet_name="", xyxy="", numberformat="#,##0.00_ "):
 		self.set_numberformat_in_range(sheet_name, xyxy, numberformat)
 
 	def set_numberformat_in_range(self, sheet_name="", xyxy="", numberformat="#,##0.00_ "):
 		"""
 		영역에 숫자형식을 지정하는 것
 		"""
@@ -3406,23 +4078,72 @@
 		rangename을 설정하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		self.xlbook.Names.Add(name, my_range)
 
+	def set_rtrim_in_range(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				value = sheet_object.Cells(y, x).Value
+				sheet_object.Cells(y, x).Value = str(value.rstrip())
+
+
+	def set_strikethrough_in_range(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		my_range.Font.Strikethrough = True
+
+	def set_swapcase_in_range(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				value = sheet_object.Cells(y, x).Value
+				sheet_object.Cells(y, x).Value = str(value.swapcase())
+
+	def set_trim_in_range(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				value = sheet_object.Cells(y, x).Value
+				sheet_object.Cells(y, x).Value = str(value.strip())
+
+
+	def set_underline_in_range(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		my_range.Font.Underline = True
+
 	def set_unmerge_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 병합된 것을 푸는 것이다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.UnMerge()
 
+	def set_upper_in_range(self, sheet_name, xyxy):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				value = sheet_object.Cells(y, x).Value
+				sheet_object.Cells(y, x).Value = str(value.upper())
+
+
 	def set_visible_for_sheet(self, input_data=0):
 		"""
 		시트를 감추는것
 		"""
 		self.xlapp.Visible = input_data
 
 	def set_visible_for_workbook(self, value=1):
@@ -3444,26 +4165,49 @@
 		"""
 		셀의 줄바꿈을 설정할때 사용한다
 		만약 status를 false로 하면 줄바꿈이 실행되지 않는다.
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.Range(xyxy).WrapText = input_data
 
+	def set_xx_width(self, sheet_name, xyxy, width=13.5):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		my_range.ColumnWidth = width
+
+
 	def show_messagebox_with_value(self, input_text="입력필요", input_title="pcell"):
 		"""
 		메세지박스를 보여주는것
 		"""
 		win32gui.MessageBox(0, input_text, input_title, 0)
 
 	def sound_beep(self, sec = 1000, hz = 500):
 		"""
 		beep 음을 내는 것
 		"""
 		win32api.Beep(hz, sec)
 
+	def split_partial_value_in_range_by_step_from_start(self, sheet_name, xyxy, n_char):
+		"""
+		어떤 자료중에 앞에서 몇번째것들만 갖고오고 싶을때
+		예:시군구 자료에서 앞의 2글자만 분리해서 얻어오는 코드
+		"""
+		list_2d = self.read_value_in_range(sheet_name, xyxy)
+		result = set()
+		for list_1d in list_2d:
+			for one in list_1d:
+				try:
+					result.add(one[0:n_char])
+				except:
+					pass
+		return list(result)
+
 	def split_value_as_engnum(self, data):
 		"""
 		 단어중에 나와있는 숫자, 영어를 분리하는기능
 		"""
 		re_compile = re.compile(r"[a-zA-Z0-9]+")
 		result = re_compile.findall(data)
 
@@ -3561,14 +4305,25 @@
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		col_list = df_obj.columns.values.tolist()
 		value_list = df_obj.values.tolist()
 		self.write_value_in_range(sheet_name, xyxy, [col_list])
 		self.write_value_in_range(sheet_name, [x1 + 1, y1], value_list)
 
+	def write_dic_key_in_cell(self, sheet_name="", xyxy="", input_dic="입력필요"):
+		"""
+		사전으로 입력된 키값을 엑셀에 쓰는것
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		changed_input_datas = list(input_dic.keys())
+
+		for x in range(0, len(changed_input_datas)):
+			sheet_object.Cells(x + x1, y1).Value = changed_input_datas[x]
+
 	def write_list1d_in_range(self, sheet_name="", xyxy="", input_list="입력필요"):
 		"""
 		1줄의 리스트는 가로로 나열된다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		if x1==x2 and y1==y2:
@@ -3608,14 +4363,18 @@
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		my_range.AddComment(text)
 
+	def write_messagebox_value(self, input_text, input_title="pcell"):
+		win32gui.MessageBox(0, input_text, input_title, 0)
+
+
 	def write_nansu_in_range(self, sheet_name="", xyxy="", input_list=[1,100]):
 		"""
 		입력한 숫자범위에서 난수를 만들어서 영역에 써주는것
 		"""
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		no_start, no_end = input_list
@@ -3627,14 +4386,30 @@
 				self.write_cell_value(sheet_name, [x, y], basic_data[temp_no])
 				if temp_no >= no_end - no_start:
 					random.shuffle(basic_data)
 					temp_no = 0
 				else:
 					temp_no = temp_no + 1
 
+	def write_range_formula(self, sheet_name, xyxy, input_data="=Now()"):
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		my_range.Formula = input_data
+	def write_serial_no_by_step(self, xyxy, start_no, step = 1):
+		"""
+		선택한 영역에 시작번호, 간격으로 이루어진 연속된 숫자를 쓰는것
+		"""
+		new_no = start_no
+		for no in range(0, xyxy[2]-xyxy[0]+1):
+			self.write_value_in_cell("", [xyxy[0]+no, xyxy[1]], new_no)
+			new_no = new_no + step
+			#print([xyxy[0]+no, xyxy[1]], new_no)
+
 	def write_value_in_activecell(self, value="입력필요"):
 		""" 활성화된 셀에 값는 넣기 """
 		self.get_activesheet_object()
 		xy = self.read_address_in_activecell()
 		self.write_value_in_cell("", [xy[0], xy[1]], value)
 
 	def write_value_in_cell(self, sheet_name="", xyxy="", value="입력필요"):
@@ -3661,25 +4436,14 @@
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		changed_input_datas = self.change_inputdata_to_list2d(input_datas)
 
 		for x in range(0, len(changed_input_datas)):
 			for y in range(0, len(changed_input_datas[x])):
 				sheet_object.Cells(x + x1, y + y1).Value = changed_input_datas[x][y]
 
-	def write_dic_key_in_cell(self, sheet_name="", xyxy="", input_dic="입력필요"):
-		"""
-		사전으로 입력된 키값을 엑셀에 쓰는것
-		"""
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		changed_input_datas = list(input_dic.keys())
-
-		for x in range(0, len(changed_input_datas)):
-			sheet_object.Cells(x + x1, y1).Value = changed_input_datas[x]
-
 	def write_value_in_range_as_speedy(self, sheet_name="", xyxy="", input_datas="입력필요"):
 		"""
 		2022-12-23 : x1, y1이 잘못되어서 변경함
 		영역과 자료의 갯수중에서 작은것을 기준으로 값을 쓰는데
 		만약 영역이 셀하나이면 자료를 전부 쓴다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
@@ -3721,15 +4485,14 @@
 			for y in range(0, y_len):
 				sheet_object.Cells(x + x1, y + y1).Value = input_datas[x][y]
 
 	def write_value_in_range_by_trans(self, sheet_name="", xyxy="", input_list2d=""):
 		"""
 		입력자료의 xy를 바꿔서 입력하는 것
 		"""
-
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				sheet_object.Cells(y, x).Value = input_list2d[x][y]
 
@@ -3742,243 +4505,29 @@
 
 		for x in range(x1, x2 + 1):
 			if divmod(x, xystep[0])[1] == 0:
 				for y in range(y1, y2 + 1):
 					if divmod(y, xystep[1])[1] == 0:
 						sheet_object.Cells(x, y).Value = str(input_text)
 
-	def open_file(self, filename=""):
-		"""
-		"""
-		self.path_full = self.check_filepath(filename)
-		self.file_name_only = self.path_full.split("/")[-1]
-		if filename.lower() == 'new'or filename == "":
-			#빈것으로 된 경우는 새로운 workbook < 연다는 뜻으로 해석
-			try:
-				self.xlapp.Windowstate = -4137
-				self.xlbook = self.xlapp.WorkBooks.Add()
-			except:
-				win32gui.MessageBox(0, "There is no Activeworkbook", "www.halmoney.com", 0)
-		else:
-				#	열린 화일중에 같은것이 있는지 확인하는 것
-				file_name_list = self.read_opened_workbook_filename_all()
-				if self.file_name_only in file_name_list:
-					pass
-				else:
-					try:
-						self.xlbook = self.xlapp.Workbooks.Open(self.path_full)
-					except:
-						win32gui.MessageBox(0, "화일이름이나 경로를 다시한번 확인해 보시기 바랍니다”, .halmoney.com", 0)
-
-	################################################################
-
-	def close_excel(self):
-		"""
-		열려진 화일을 닫는것
-		"""
-		self.xlbook.Close(SaveChanges=0)
-		del self.xlapp
-
-	def close_activeworkbook(self):
-		"""
-		열려진 화일을 닫는것
-		"""
-		self.xlbook.Close(SaveChanges=0)
-
-	def change_active_workbook(self, input_file_name):
-		"""
-		열려진 워드 화일중 이름으로 선택하는것
-		"""
-		self.xlapp.Visible = True
-		win32gui.SetForegroundWindow(self.xlapp.hwnd)
-		self.xlapp.WorkBooks(input_file_name).Activate()
-		self.xlapp.WindowState = win32com.client.constants.xlMaximized
-
-	def make_password(self, isnum="yes", istext_small="yes", istext_big="yes", isspecial="no", len_num=10):
-		"""
-		엑셀시트의 암호를 풀기위해 암호를 계속 만들어서 확인하는 것
-		"""
-		check_char = []
-		if isnum == "yes":
-			check_char.extend(list(string.digits))
-		if istext_small == "yes":
-			check_char.extend(list(string.ascii_lowercase))
-		if istext_big == "yes":
-			check_char.extend(list(string.ascii_uppercase))
-		if isspecial == "yes":
-			for one in "!@#$%^*_-":
-				check_char.extend(one)
-
-		zz = combinations_with_replacement(check_char, len_num)
-		for aa in zz:
-			try:
-				pswd = "".join(aa)
-				#print(pswd)
-				self.unlock_sheet("", pswd)
-				break
-				#print("발견", pswd)
-			except:
-				pass
-
-
-	def check_same_data(self, input_list, check_line = 10):
-		"""
-		엑셀의 선택한 자료에서 여러줄을 기준으로 같은 자료만 갖고오기
-		"""
-		result = []
-		base_value = ""
-		xy = self.read_address_in_activecell()
-		for no in input_list:
-			base_value = base_value + str(self.read_cell_value("", [xy[0], no]))
-
-		# 혹시 1보다 작은 숫자가 나올 수있으므로, 최소시작점을 1로하기위해
-		start_x = max(int(xy[0]) - check_line, 1)
-
-		# 위로10개 아래로 10개의 자료를 확인한다
-		for no in range(start_x, start_x+20):
-			cell_value=""
-			for one in input_list:
-				cell_value = cell_value + str(self.read_cell_value("", [no, one]))
-			if base_value == cell_value:
-				# 보통 50개이상의 줄을 사용하지 않으므로 50개를 갖고온다
-				temp = self.read_value_in_range("", [no, 1, no, 50])
-				result.append(temp[0])
-		return result
-
-	def check_differ_at_same_area(self, input_sa1, input_sa2):
-		"""
-		동일한 사이즈의 다른 영역에서 다른 것만 색칠하기
-		"""
-		datal = self.read_value_in_range(input_sa1[0], input_sa1[1])
-		data2 = self.read_value_in_range(input_sa2[0], input_sa2[1])
-		start_x = input_sa2[1][0]
-		start_y = input_sa2[1][1]
-		for x in range(len(datal)):
-			for y in range(len(datal[0])):
-				if datal[x][y] == data2[x][y]:
-					pass
-				else:
-					self.paint_cell_by_excel_colorno(input_sa2[0], [x + start_x, y + start_y], 3)
+	def write_value_to_left(self, input_text=""):
+		cell_value = vars["cell"].Value
+		vars["cell"].Value = str(input_text) + str(cell_value[0])
+
+	def make_xy_list_for_box_style(self, xyxy):
+		# 좌표를 주면, 맨끝만 나터내는 좌표를 얻는다
+		temp_1 = []
+		for x in [xyxy[0], xyxy[2]]:
+			temp = []
+			for y in range(xyxy[1], xyxy[3] + 1):
+				temp.append([x, y])
+			temp_1.append(temp)
+
+		temp_2 = []
+		for y in [xyxy[1], xyxy[3]]:
+			temp = []
+			for x in range(xyxy[0], xyxy[2] + 1):
+				temp.append([x, y])
+			temp_2.append(temp)
 
-	def concate_xlne(self, input_list2d, xy):
-		"""
-		# 선택한 영역의 세로자료들을 다 더해서 제일위의 셀에 다시 넣는것
-		"""
-		x_len = len(input_list2d)
-		y_len = len(input_list2d[0])
-		for y in range(y_len):
-			temp = ""
-			for x in range(x_len):
-				self.write_value_in_cell("", [x + xy[0], y + xy[1]], "")
-				if input_list2d[x][y]:
-					#print(input_list2d[x][y])
-					temp = temp + " " + input_list2d[x][y]
-			#print(temp)
-			self.write_value_in_cell("", [xy[0], y + xy[1]], str(temp).strip())
-
-	def write_serial_no_by_step(self, xyxy, start_no, step = 1):
-		"""
-		선택한 영역에 시작번호, 간격으로 이루어진 연속된 숫자를 쓰는것
-		"""
-		new_no = start_no
-		for no in range(0, xyxy[2]-xyxy[0]+1):
-			self.write_value_in_cell("", [xyxy[0]+no, xyxy[1]], new_no)
-			new_no = new_no + step
-			#print([xyxy[0]+no, xyxy[1]], new_no)
-
-	def split_partial_value_in_range_by_step_from_start(self, sheet_name, xyxy, n_char):
-		"""
-		어떤 자료중에 앞에서 몇번째것들만 갖고오고 싶을때
-		예:시군구 자료에서 앞의 2글자만 분리해서 얻어오는 코드
-		"""
-		list_2d = self.read_value_in_range(sheet_name, xyxy)
-		result = set()
-		for list_1d in list_2d:
-			for one in list_1d:
-				try:
-					result.add(one[0:n_char])
-				except:
-					pass
-		return list(result)
-
-	def rotate_shape(self, sheet_name, shape_obj, degree):
-		# 도형을 회전시키는 것
-		# shape _ obi :이동시킬 도형 이름
-		sheet_object = self.check_sheet_name(sheet_name)
-		oShape = sheet_object.Shapes(shape_obj)
-		oShape.IncrementRotation(degree)
-
-	def read_all_shape_names(self, sheet_name=""):
-		sheet_object = self.check_sheet_name(sheet_name)
-		drawings_nos = sheet_object.Shapes.count
-		result = []
-		if drawings_nos > 0:
-			for num in range(sheet_object.Shapes.count, 0, -1):
-				# Range를 앞에서부터하니 삭제하자마자 번호가 다시 매겨져서, 뒤에서부터 삭제하니 잘된다
-				result.append(sheet_object.Shapes(num).Name)
-		return result
-
-	def move_shape(self, sheet_name, shape_obj, top, left):
-		# shape_0b] : 이동시림 도형 이름
-		sheet_object = self.check_sheet_name(sheet_name)
-		oShape = sheet_object.Shapes(shape_obj)
-		oShape.Top = oShape.Top + top
-		oShape.Left = oShape.left + left
-
-	def add_shape(self, sheet_name, shape_no=35, xywh=""):
-		# shape_no : 엑셀에서 정의한 도형의 번호
-		# xywh : 왼쪽윗부분의 위치에서 너비와 높이
-		sheet_object = self.check_sheet_name(sheet_name)
-
-		#도형이 숫자이면 그대로, 문자이면 기본자료에서 찾도록 한다
-		if type(shape_no) == type(123):
-			pass
-		elif shape_no in list(self.data_set_basic.vars["shape_enum"].keys()):
-			shape_no = self.data_set_basic.vars["shape_enum"][shape_no]
-
-		sheet_object.Shapes.Addshape(shape_no, xywh[0], xywh[1], xywh[2], xywh[3])
-
-	def get_xy_list_for_circle(self, r, precious=10, xy=[0, 0]):
-		# 엑셀을 기준으로, 반지름이 글자를 원으로 계속 이동시키는 것
-		# r;반지름
-		# precious : 얼마나 정밀하게 할것인지, 1도를 몇번으로 나누어서 계산할것인지
-		result = []
-		temp = []
-		for do_1 in range(1, 5):
-			for do_step in range(90 * precious + 1):
-				degree = (do_1 * do_step) / precious
-				# r을 더하는 이유는 마이너스는 않되므로 x, y측을 이동시키는것
-				x = math.cos(degree) * r
-				y = math.sin(degree) * r
-				new_xy = [int(round(x)), int(round(y))]
-
-				if not new_xy in temp:
-					temp.append(new_xy)
-		area_1 = []
-		area_2 = []
-		area_3 = []
-		area_4 = []
-
-		for x, y in temp:
-			new_x = x + r + 1 + xy[0]
-			new_y = y + r + 1 + xy[1]
-
-			if x >= 0 and y >= 0:
-				area_1.append([new_x, new_y])
-			elif x >= 0 and y < 0:
-				area_2.append([new_x, new_y])
-			elif x < 0 and y < 0:
-				area_3.append([new_x, new_y])
-			elif x < 0 and y >= 0:
-				area_4.append([new_x, new_y])
-		area_1.sort()
-		area_1.reverse()
-		area_2.sort()
-		area_3.sort()
-		area_4.sort()
-		area_4.reverse()
-
-		result.extend(area_2)
-		result.extend(area_1)
-		result.extend(area_4)
-		result.extend(area_3)
+		result = [temp_1[0], temp_2[1], temp_1[1], temp_2[0]]
 		return result
```

### Comparing `xython-1.3.0/src/xython/pcell_event.py` & `xython-1.4.0/src/xython/pcell_event.py`

 * *Files identical despite different names*

### Comparing `xython-1.3.0/src/xython/pyclick.py` & `xython-1.4.0/src/xython/pyclick.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 # -*- coding: utf-8 -*-
 import time  #내장모듈
 
-import pyperclip
+import basic_data  # xython 모듈
+
+import pyperclip3
 import pyautogui
 
 class pyclick:
 	"""
 	여러가지 사무용에 사용할 만한 메소드들을 만들어 놓은것이며,
 	좀더 특이한 것은 youtil2로 만들어서 사용할 예정입니다 
 	"""
-	#def __init__(self):
-	#공통으로 사용할 변수들을 설정하는 것
-	#keyboard.wait('esc')  # esc 키를 누를때 까지 대기합니다.
 
+	def __init__(self):
+		self.base_data = basic_data.basic_data()
+		self.var = self.base_data.vars
+		self.var_common={}
 
 	def check_action_key(self, input_value):
-		action_key_list = [
-		'f1', 'f10', 'f11', 'f12', 'f2', 'f3', 'f4', 'f5', 'f6', 'f7', 'f8', 'f9',	'fn',
-		'left', 'right','up', 'down','end', 'home','space', 'tab',
-		'alt', 'altleft', 'altright', 'ctrl', 'ctrlleft', 'ctrlright','shift', 'shiftleft', 'shiftright', 'win', 'winleft', 'winright',
-		'capslock', 'del', 'delete','backspace', 'enter', 'esc', 'escape', 'insert','numlock',
-		'pagedown', 'pageup', 'pgdn', 'pgup',
-		'hanguel', 'hangul', 'hanja',
-		'printscreen', 'prtscr',
-		]
 		input_value = str(input_value).lower()
-		if input_value in action_key_list:
+		if input_value in self.var["action_key_list"]:
 			result = input_value
 		else:
 			result = ""
 		return result
 
 	def click_mouse_general(self, click_type="click", click_times=1, interval_time=0.25):
 		# 마우스 클릭에 대한 일반적인것
@@ -54,36 +48,16 @@
 	def click_mouse_right_up(self):
 		pyautogui.mouseUp(button='right')
 
 	def copy(self):
 		pyautogui.hotkey('ctrl', "c")
 
 	def data_keyboard(self):
-		result =['\\t', '\\n', '\\r', ' ', '!', '"', '#', '$', '%', '&', "'", '(',
-				')', '*', '+', ',', '-', '.', '/', '0', '1', '2', '3', '4', '5', '6', '7',
-				'8', '9', ':', ';', '<', '=', '>', '?', '@', '[', '\\', ']', '^', '_', '`',
-				'a', 'b', 'c', 'd', 'e','f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o',
-				'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', '{', '|', '}', '~',
-				'accept', 'add', 'alt', 'altleft', 'altright', 'apps', 'backspace',
-				'browserback', 'browserfavorites', 'browserforward', 'browserhome',
-				'browserrefresh', 'browsersearch', 'browserstop', 'capslock', 'clear',
-				'convert', 'ctrl', 'ctrlleft', 'ctrlright', 'decimal', 'del', 'delete',
-				'divide', 'down', 'end', 'enter', 'esc', 'escape', 'execute', 'f1', 'f10',
-				'f11', 'f12', 'f13', 'f14', 'f15', 'f16', 'f17', 'f18', 'f19', 'f2', 'f20',
-				'f21', 'f22', 'f23', 'f24', 'f3', 'f4', 'f5', 'f6', 'f7', 'f8', 'f9',
-				'final', 'fn', 'hanguel', 'hangul', 'hanja', 'help', 'home', 'insert', 'junja',
-				'kana', 'kanji', 'launchapp1', 'launchapp2', 'launchmail',
-				'launchmediaselect', 'left', 'modechange', 'multiply', 'nexttrack',
-				'nonconvert', 'num0', 'num1', 'num2', 'num3', 'num4', 'num5', 'num6',
-				'num7', 'num8', 'num9', 'numlock', 'pagedown', 'pageup', 'pause', 'pgdn',
-				'pgup', 'playpause', 'prevtrack', 'print', 'printscreen', 'prntscrn',
-				'prtsc', 'prtscr', 'return', 'right', 'scrolllock', 'select', 'separator',
-				'shift', 'shiftleft', 'shiftright', 'sleep', 'space', 'stop', 'subtract', 'tab',
-				'up', 'volumedown', 'volumemute', 'volumeup', 'win', 'winleft', 'winright', 'yen',
-				'command', 'option', 'optionleft', 'optionright']
+
+		result =self.var["keyboard_action_list_all"]
 		return result
 
 	def double_click_mouse_left(self, interval_time=0.25):
 		pyautogui.click(button="left", clicks=2, interval=interval_time)
 
 	def double_click_mouse_right(self, interval_time=0.25):
 		pyautogui.click(button="right", clicks=2, interval=interval_time)
@@ -136,15 +110,15 @@
 		print(a)
 
 	def paste(self):
 		pyautogui.hotkey('ctrl', "v")
 
 	def paste_for_clibboard_data(self):
 		# 클립보드에 저장된 텍스트를 붙여넣습니다.
-		pyperclip.paste()
+		pyperclip3.paste()
 
 	def press_one_key(self, input_key="enter"):
 		#기본적인 키를 누르는 것을 설정하는 것이며
 		#기본값은 enter이다
 		#press의 의미는 down + up이다
 		pyautogui.press(input_key)
 
@@ -246,39 +220,37 @@
 	def type_hotkey_n_key(self, input_hotkey, input_key):
 		# pyautogui.hotkey(’ctrl’, *c') ==> ctrl-c to copy
 		pyautogui.hotkey(input_hotkey, input_key)
 
 	def type_text_for_hangul(self, input_text):
 		# 영문은 어떻게 하면 입력이 잘되는데, 한글이나 유니코드는 잘되지 않아 찾아보니 아래의 형태로 사용하시면 가능합니다
 		# pyautogui 가 unicode 는 입력이 안됩니다
-		pyperclip.copy(input_text)
+		pyperclip3.copy(input_text)
 		pyautogui.hotkey('ctrl', "v")
 
 	def type_text_one_by_one(self, input_text):
 		# 영문은 어떻게 하면 입력이 잘되는데, 한글이나 유니코드는 잘되지 않아 찾아보니 아래의 형태로 사용하시면 가능합니다
 		# 어떤경우는 여러개는 않되어서 한개씩 들어가는 형태로 한다
 		for one_letter in input_text:
-			pyperclip.copy(one_letter)
+			pyperclip3.copy(one_letter)
 			pyautogui.hotkey("ctrl", "v")
 
 	def type_text_with_interval(self, input_text, input_interval=0.1):
 		# 그저 글자를 타이핑 치는 것이다
 		# pyautogui.pressfenter', presses=3z interval=3) # enter 키를 3 초에 한번씩 세번 입력합니다.
 		pyautogui.typewrite(input_text, interval=input_interval)
 
-#########################################################################
-
 	def type_ctrl_plus_letter(self, input_text):
 		pyautogui.hotkey('ctrl', input_text)
 
 	def type_normal_key(self, input_text="enter"):
 		pyautogui.press(input_text)
 
 	def mouse_drag(self, pxy):
 		pyautogui.dragTo(pxy[0], pxy[1])
 
 	def get_text_from_clipboard(self):
 		"""
 		클립보드에 입력된 내용을 복사를 하는 것이다
 		"""
-		result = pyperclip.paste()
+		result = pyperclip3.paste()
 		return result
```

### Comparing `xython-1.3.0/src/xython/scolor.py` & `xython-1.4.0/src/xython/scolor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,190 +1,36 @@
 # -*- coding: utf-8 -*-
 import re  #내장모듈
 
-import basic_data  # halmoney 모듈
+import basic_data  # xython 모듈
 
 class scolor:
 	"""
 	색을 쉽게 사용하기위해 만든 모듈
 	"""
 	def __init__(self):
-		color_data = basic_data.basic_data()
-		self.color_vars = color_data.vars
+		self.base_data = basic_data.basic_data()
+		self.var = self.base_data.vars
+		self.var_common={}
+
 
 	def change_color_to_hsl(self, input_scolor):
 		result = self.change_scolor_to_hsl(input_scolor)
 		return result
 
 	def change_color_to_rgb(self, input_scolor):
 		hsl_value = self.change_scolor_to_hsl(input_scolor)
 		result = self.change_hsl_to_rgb(hsl_value)
 		return result
 
-	def data_basic_color_step(self):
-		result = self.color_vars["basic_color_step"]
-		return result
-
-
-	def change_scolor_to_rgb_with_style(self, input_scolor="red45", color_style="파스텔", style_step=5):
-		"""
-		입력된 기본 값을 스타일에 맞도록 바꾸고, 스타일을 강하게 할것인지 아닌것인지를 보는것
-		color_style : pccs의 12가지 사용가능, 숫자로 사용가능, +-의 형태로도 사용가능
-		입력예 : 기본색상, 적용스타일, 변화정도,("red45, 파스텔, 3)
-		변화정도는 5를 기준으로 1~9까지임
-		"""
-		# 넘어온 자료중 color값을 hsl로 변경한다
-		basic_hsl = self.change_scolor_to_hsl(input_scolor)
-		# 스타일을 적용하는것
-		aaa = self.color_vars["color_tone_12_names_vs_no"][color_style]
-		step_2 = self.color_vars["sl_small_step_vs_sl_no"][aaa]
-		# 스타일을 얼마나 강하게 적용할것인가를 나타내는것
-		step_1 = self.color_vars["sl_big_step_vs_sl_no"][str(style_step)]
-
-		h = int(basic_hsl[0])
-		s = int(basic_hsl[1]) + int(step_1[0]) + int(step_2[0])
-		l = int(basic_hsl[2]) + int(step_1[1]) + int(step_2[1])
-
-		changed_rgb = self.change_hsl_to_rgb([h, s, l])
-		return changed_rgb
-
 	def change_excel56_to_rgb(self, input_no):
 		"""
 		엑셀 기본 rgb 색 : 56색
 		"""
-		result = self.color_vars["rgb_56_for_excel"][int(input_no)]
-		return result
-
-	def change_hsl_to_rgb_by_change_mode(self, hsl_value, change_mode):
-		"""
-		change_mode : ++, --, 70등의 값이 들어오면 변화를 시켜주는 것
-		"""
-		if type(change_mode) == type(123):
-			#50을 기본으로 차이나는 부분을 계산하는것
-			l_value = change_mode - 50
-			if l_value < 0:
-				l_value = 0
-		elif "+" == str(change_mode)[0]:
-			# 현재의 값에서 10만큼 밝아지도록 한다
-			l_value = 10 * len(change_mode)
-		elif "-" == str(change_mode)[0]:
-			# 현재의 값에서 10만큼 어두워지도록 한다
-			l_value = -10 * len(change_mode)
-
-		final_l_value = hsl_value[2] + l_value
-		if final_l_value > 100 :
-			final_l_value = 100
-		elif final_l_value < 0 :
-			final_l_value = 0
-
-		result = [hsl_value[0], hsl_value[1], final_l_value]
-		return result
-
-	def change_hsl_to_rgb_by_high_l(self, hsl, high_l = 80):
-		"""
-		고명도의 hsl로 변경
-		"""
-		result = self.change_hsl_to_rgb([hsl[0], hsl[1], high_l])
-		return [result]
-
-	def change_hsl_to_rgb_by_high_s(self, hsl, high_s = 80):
-		#고채도
-		result = self.change_hsl_to_rgb([hsl[0], high_s, hsl[2]])
-		return [result]
-
-	def change_hsl_to_rgb_by_low_l(self, hsl, high_l = 20):
-		"""
-		저명도, 20%정도의 명도를 저명도로 말하자자
-		"""
-		result = self.change_hsl_to_rgb([hsl[0], hsl[1], high_l])
-		return [result]
-
-	def change_hsl_to_rgb_by_low_s(self, hsl, high_s = 20):
-		#저채도
-		result = self.change_hsl_to_rgb([hsl[0], high_s, hsl[2]])
-		return [result]
-
-	def change_hsl_to_rgb_by_middle_l(self, hsl, high_l = 50):
-		"""
-		중명도의 hsl로 변경
-		"""
-		result = self.change_hsl_to_rgb([hsl[0], hsl[1], high_l])
-		return [result]
-
-	def change_hsl_to_rgb_by_middle_s(self, hsl, high_s = 50):
-		#중채도
-		result = self.change_hsl_to_rgb([hsl[0], high_s, hsl[2]])
-		return [result]
-
-	def change_hsl_to_rgb_with_near_10_color_set(self, hsl, step = 10):
-		"""
-		위쪽으로 5개, 아래로 5개의 채도가 비슷한 색을 돌려준다
-		채도의 특성상 비슷한 부분이 많아서 10단위로 만든다
-		"""
-		h, s, l = hsl
-		result = []
-		for no in range(0,100+step,step):
-			#print("변경된 hsl은 s=> ", [h, no, l])
-			temp = self.change_hsl_to_rgb([h, no, l])
-			result.append(temp)
-		return result
-
-	def change_hsl_to_rgb_with_20_hsl_by_l_step(self, hsl):
-		"""
-		위쪽으로 5개, 아래로 5개의 명도가 비슷한 색을 돌려준다
-		"""
-		h, s, l = hsl
-		result = []
-		for no in range(0, 21):
-			temp = self.change_hsl_to_rgb([h, s, no * 5])
-			result.append(temp)
-		return result
-
-	def change_hsl_to_rgb_with_20_hsl_by_s_step(self, hsl):
-		"""
-		위쪽으로 5개, 아래로 5개의 명도가 비슷한 색을 돌려준다
-		"""
-		h, s, l = hsl
-		result = []
-		for no in range(0, 21):
-			temp = self.change_hsl_to_rgb([h, no*5, l])
-			result.append(temp)
-		return result
-
-	def change_hsl_to_3rgb_by_2near_bo_style(self, hsl, h_step=36):
-		"""
-		근접보색조합 : 보색의 양쪽 근처색
-		분열보색조합 : Split Complementary
-		근접보색조합이라고도 한다. 보색의 강한 인상이 부담스러울때 보색의 근처에 있는 색을 사용
-		2차원 list의 형태로 돌려줌
-		"""
-		h, s, l = hsl
-
-		new_h_1 = divmod(h - h_step + 180, 360)[1]
-		new_h_3 = divmod(h + h_step + 180, 360)[1]
-		rgb_1 = self.change_hsl_to_rgb([new_h_1, s, l])
-		rgb_2 = self.change_hsl_to_rgb(hsl)
-		rgb_3 = self.change_hsl_to_rgb([new_h_3, s, l])
-		result = [rgb_1, rgb_2, rgb_3]
-
-		return result
-
-	def change_hsl_to_3rgb_by_2near_style (self, hsl, h_step=36):
-		"""
-		근접색조합 : 양쪽 근처색
-		"""
-		h, s, l = hsl
-
-		new_h_1 = divmod(h - h_step, 360)[1]
-		new_h_3 = divmod(h + h_step, 360)[1]
-
-		rgb_1 = self.change_hsl_to_rgb([new_h_1, s, l])
-		rgb_2 = self.change_hsl_to_rgb(hsl)
-		rgb_3 = self.change_hsl_to_rgb([new_h_3, s, l])
-		result = [rgb_1, rgb_2, rgb_3]
+		result = self.var["rgb_56_for_excel"][int(input_no)]
 		return result
 
 	def change_hsl_to_36_hsl_by_h_step(self, hsl):
 		"""
 		위쪽으로 5개, 아래로 5개의 명도가 비슷한 색을 돌려준다
 		"""
 		h, s, l = hsl
@@ -244,56 +90,46 @@
 		new_h_3 = divmod(h + h_step + 180, 360)[1]
 
 		hsl_1 = [new_h_1, s, l]
 		hsl_3 = [new_h_3, s, l]
 		result_rgb = self.change_hsl_to_rgb([hsl_1, hsl, hsl_3])
 		return result_rgb
 
-	def change_hsl_to_rgb_for_4_tetra_style(self, hsl):
+	def change_hsl_to_3rgb_by_2near_bo_style(self, hsl, h_step=36):
 		"""
-		4가지 꼭지의
+		근접보색조합 : 보색의 양쪽 근처색
+		분열보색조합 : Split Complementary
+		근접보색조합이라고도 한다. 보색의 강한 인상이 부담스러울때 보색의 근처에 있는 색을 사용
+		2차원 list의 형태로 돌려줌
 		"""
 		h, s, l = hsl
 
-		new_h_1 = divmod(h + 0, 360)[1]
-		new_h_2 = divmod(h + 90, 360)[1]
-		new_h_3 = divmod(h + 180, 360)[1]
-		new_h_4 = divmod(h + 270, 360)[1]
+		new_h_1 = divmod(h - h_step + 180, 360)[1]
+		new_h_3 = divmod(h + h_step + 180, 360)[1]
 		rgb_1 = self.change_hsl_to_rgb([new_h_1, s, l])
-		rgb_2 = self.change_hsl_to_rgb([new_h_2, s, l])
+		rgb_2 = self.change_hsl_to_rgb(hsl)
 		rgb_3 = self.change_hsl_to_rgb([new_h_3, s, l])
-		rgb_4 = self.change_hsl_to_rgb([new_h_4, s, l])
-		result = [rgb_1, rgb_2, rgb_3, rgb_4]
+		result = [rgb_1, rgb_2, rgb_3]
 
 		return result
 
-	def change_hsl_to_rgb_for_bo_style(self, hsl):
-		"""
-		입력된 hsl의 보색을 알려주는것
-		보색 : Complementary
-		2차원 list의 형태로 돌려줌
-		"""
-		h, s, l = hsl
-		new_h = divmod(h+180, 360)[1]
-		result = self.change_hsl_to_rgb([new_h, s, l])
-		return [result]
-
-	def change_hsl_to_rgb_for_bo_style_1(self, hsl):
+	def change_hsl_to_3rgb_by_2near_style (self, hsl, h_step=36):
 		"""
-		mode : 1
-		보색 : Complementary
+		근접색조합 : 양쪽 근처색
 		"""
 		h, s, l = hsl
 
-		new_h_1 = h + 180
-		if new_h_1 >= 360:
-			new_h_1 = 360 - new_h_1
+		new_h_1 = divmod(h - h_step, 360)[1]
+		new_h_3 = divmod(h + h_step, 360)[1]
 
-		result_rgb = self.change_hsl_to_rgb([new_h_1, s, l])
-		return result_rgb
+		rgb_1 = self.change_hsl_to_rgb([new_h_1, s, l])
+		rgb_2 = self.change_hsl_to_rgb(hsl)
+		rgb_3 = self.change_hsl_to_rgb([new_h_3, s, l])
+		result = [rgb_1, rgb_2, rgb_3]
+		return result
 
 	def change_hsl_to_rgb(self, hsl):
 		"""
 		hsl을 rgb로 바꾸는 것이다
 		"""
 		#print("hsl값은 ==> ", hsl)
 		h, s, l = hsl
@@ -361,25 +197,180 @@
 		R = int(abs(round(R * 255,0)))
 		G = int(abs(round(G * 255,0)))
 		B = int(abs(round(B * 255,0)))
 
 		#rgb_to_int = (int(B)) * (256 ** 2) + (int(G)) * 256 + int(R)
 		return [R, G, B]
 
+	def change_hsl_to_rgb_by_change_mode(self, hsl_value, change_mode):
+		"""
+		change_mode : ++, --, 70등의 값이 들어오면 변화를 시켜주는 것
+		"""
+		if type(change_mode) == type(123):
+			#50을 기본으로 차이나는 부분을 계산하는것
+			l_value = change_mode - 50
+			if l_value < 0:
+				l_value = 0
+		elif "+" == str(change_mode)[0]:
+			# 현재의 값에서 10만큼 밝아지도록 한다
+			l_value = 10 * len(change_mode)
+		elif "-" == str(change_mode)[0]:
+			# 현재의 값에서 10만큼 어두워지도록 한다
+			l_value = -10 * len(change_mode)
+
+		final_l_value = hsl_value[2] + l_value
+		if final_l_value > 100 :
+			final_l_value = 100
+		elif final_l_value < 0 :
+			final_l_value = 0
+
+		result = [hsl_value[0], hsl_value[1], final_l_value]
+		return result
+
+	def change_hsl_to_rgb_by_high_l(self, hsl, high_l = 80):
+		"""
+		고명도의 hsl로 변경
+		"""
+		result = self.change_hsl_to_rgb([hsl[0], hsl[1], high_l])
+		return [result]
+
+	def change_hsl_to_rgb_by_high_s(self, hsl, high_s = 80):
+		#고채도
+		result = self.change_hsl_to_rgb([hsl[0], high_s, hsl[2]])
+		return [result]
+
+	def change_hsl_to_rgb_by_low_l(self, hsl, high_l = 20):
+		"""
+		저명도, 20%정도의 명도를 저명도로 말하자자
+		"""
+		result = self.change_hsl_to_rgb([hsl[0], hsl[1], high_l])
+		return [result]
+
+	def change_hsl_to_rgb_by_low_s(self, hsl, high_s = 20):
+		#저채도
+		result = self.change_hsl_to_rgb([hsl[0], high_s, hsl[2]])
+		return [result]
+
+	def change_hsl_to_rgb_by_middle_l(self, hsl, high_l = 50):
+		"""
+		중명도의 hsl로 변경
+		"""
+		result = self.change_hsl_to_rgb([hsl[0], hsl[1], high_l])
+		return [result]
+
+	def change_hsl_to_rgb_by_middle_s(self, hsl, high_s = 50):
+		#중채도
+		result = self.change_hsl_to_rgb([hsl[0], high_s, hsl[2]])
+		return [result]
+
+	def change_hsl_to_rgb_by_triangle_style(self, hsl):
+		"""
+		등간격 3색조합 : triad
+		활동적인 인상과 이미지를 보인다
+		"""
+		h, s, l = hsl
+
+		new_h_1 = divmod(h + 120, 360)[1]
+		new_h_3 = divmod(h + 240, 360)[1]
+
+		rgb_1 = self.change_hsl_to_rgb([new_h_1, s, l])
+		rgb_2 = self.change_hsl_to_rgb(hsl)
+		rgb_3 = self.change_hsl_to_rgb([new_h_3, s, l])
+		result = [rgb_1, rgb_2, rgb_3]
+		return result
+
+	def change_hsl_to_rgb_for_4_tetra_style(self, hsl):
+		"""
+		4가지 꼭지의
+		"""
+		h, s, l = hsl
+
+		new_h_1 = divmod(h + 0, 360)[1]
+		new_h_2 = divmod(h + 90, 360)[1]
+		new_h_3 = divmod(h + 180, 360)[1]
+		new_h_4 = divmod(h + 270, 360)[1]
+		rgb_1 = self.change_hsl_to_rgb([new_h_1, s, l])
+		rgb_2 = self.change_hsl_to_rgb([new_h_2, s, l])
+		rgb_3 = self.change_hsl_to_rgb([new_h_3, s, l])
+		rgb_4 = self.change_hsl_to_rgb([new_h_4, s, l])
+		result = [rgb_1, rgb_2, rgb_3, rgb_4]
+
+		return result
+
+	def change_hsl_to_rgb_for_bo_style(self, hsl):
+		"""
+		입력된 hsl의 보색을 알려주는것
+		보색 : Complementary
+		2차원 list의 형태로 돌려줌
+		"""
+		h, s, l = hsl
+		new_h = divmod(h+180, 360)[1]
+		result = self.change_hsl_to_rgb([new_h, s, l])
+		return [result]
+
+	def change_hsl_to_rgb_for_bo_style_1(self, hsl):
+		"""
+		mode : 1
+		보색 : Complementary
+		"""
+		h, s, l = hsl
+
+		new_h_1 = h + 180
+		if new_h_1 >= 360:
+			new_h_1 = 360 - new_h_1
+
+		result_rgb = self.change_hsl_to_rgb([new_h_1, s, l])
+		return result_rgb
+
+	def change_hsl_to_rgb_with_20_hsl_by_l_step(self, hsl):
+		"""
+		위쪽으로 5개, 아래로 5개의 명도가 비슷한 색을 돌려준다
+		"""
+		h, s, l = hsl
+		result = []
+		for no in range(0, 21):
+			temp = self.change_hsl_to_rgb([h, s, no * 5])
+			result.append(temp)
+		return result
+
+	def change_hsl_to_rgb_with_20_hsl_by_s_step(self, hsl):
+		"""
+		위쪽으로 5개, 아래로 5개의 명도가 비슷한 색을 돌려준다
+		"""
+		h, s, l = hsl
+		result = []
+		for no in range(0, 21):
+			temp = self.change_hsl_to_rgb([h, no*5, l])
+			result.append(temp)
+		return result
+
+	def change_hsl_to_rgb_with_near_10_color_set(self, hsl, step = 10):
+		"""
+		위쪽으로 5개, 아래로 5개의 채도가 비슷한 색을 돌려준다
+		채도의 특성상 비슷한 부분이 많아서 10단위로 만든다
+		"""
+		h, s, l = hsl
+		result = []
+		for no in range(0,100+step,step):
+			#print("변경된 hsl은 s=> ", [h, no, l])
+			temp = self.change_hsl_to_rgb([h, no, l])
+			result.append(temp)
+		return result
+
 	def change_hsl_to_rgb_with_style(self, input_color, color_style, style_step=5):
 		"""
 		입력된 기본 값을 스타일에 맞도록 바꾸는것
 		스타일을 강하게 할것인지 아닌것인지를 보는것
 		입력예 : 기본색상, 적용스타일, 변화정도, "red45, 파스텔, 3
 		변화정도는 5를 기준으로 1~9까지임
 		"""
 		basic_hsl = input_color
-		aaa = self.color_vars["check_change_step"][color_style]
-		step_1 = self.color_vars["sl_big_step_vs_sl_no"] [str(aaa)]
-		step_2 = self.color_vars["sl_small_step_vs_sl_no"] [str(style_step)]
+		aaa = self.var["check_change_step"][color_style]
+		step_1 = self.var["sl_big_step_vs_sl_no"] [str(aaa)]
+		step_2 = self.var["sl_small_step_vs_sl_no"] [str(style_step)]
 
 		h = int(basic_hsl[0])
 		s = int(basic_hsl[1]) + int(step_1[0]) + int(step_2[0])
 		l = int(basic_hsl[2]) + int(step_1[1]) + int(step_2[1])
 
 		changed_rgb = self.change_hsl_to_rgb([h, s, l])
 		return changed_rgb
@@ -388,41 +379,25 @@
 		"""
 		입력된 기본 값을 스타일에 맞도록 바꾸고, 스타일을 강하게 할것인지 아닌것인지를 보는것
 		color_style : pccs의 12가지 사용가능, 숫자로 사용가능, +-의 형태로도 사용가능
 		입력예 : 기본색상, 적용스타일, 변화정도,("red45, 파스텔, 3)
 		변화정도는 5를 기준으로 1~9까지임
 		"""
 
-		step = self.color_vars["color_tone_12_names_vs_no"][color_style]
-		step_2 = self.color_vars["sl_big_step_vs_sl_no"][step] # 스타일을 적용하는것
-		step_1 = self.color_vars["sl_small_step_vs_sl_no"][str(style_step)] # 스타일을 얼마나 강하게 적용할것인가를 나타내는것
+		step = self.var["color_tone_12_names_vs_no"][color_style]
+		step_2 = self.var["sl_big_step_vs_sl_no"][step] # 스타일을 적용하는것
+		step_1 = self.var["sl_small_step_vs_sl_no"][str(style_step)] # 스타일을 얼마나 강하게 적용할것인가를 나타내는것
 
 		h = int(input_hsl[0])
 		s = int(step_1[0]) + int(step_2[0])
 		l = int(step_1[1]) + int(step_2[1])
 
 		changed_rgb = self.change_hsl_to_rgb([h, s, l])
 		return changed_rgb
 
-	def change_hsl_to_rgb_by_triangle_style(self, hsl):
-		"""
-		등간격 3색조합 : triad
-		활동적인 인상과 이미지를 보인다
-		"""
-		h, s, l = hsl
-
-		new_h_1 = divmod(h + 120, 360)[1]
-		new_h_3 = divmod(h + 240, 360)[1]
-
-		rgb_1 = self.change_hsl_to_rgb([new_h_1, s, l])
-		rgb_2 = self.change_hsl_to_rgb(hsl)
-		rgb_3 = self.change_hsl_to_rgb([new_h_3, s, l])
-		result = [rgb_1, rgb_2, rgb_3]
-		return result
-
 	def change_input_value_to_hsl(self, input_value):
 		"""
 		입력되는 형태에 따라서 hsl을 돌려주는것
 		입력값 : rgb형식, hsl형식, scolor형식
 		결과값 : hsl값
 		"""
 		if type(input_value) == type("string"): #문자열 형식일때 scolor형식으로 해석
@@ -447,15 +422,15 @@
 		"""
 		pccs : 일본색체연구서가 빌표한 12가지 색으로 구분한것
 		어떤 입력된 색의 기본적인 PCSS 12색을 돌려준다
 		pccs톤, rgb로 넘어온 색을 pcss톤 12개로 만들어서 돌려준다
 		"""
 		result = []
 		h, s, l = self.change_rgb_to_hsl(rgb)
-		result4 = self.color_vars["color_name_for_basic_12_eng"]
+		result4 = self.var["color_name_for_basic_12_eng"]
 		for one in result4:
 			result.append([h, one[0], one[1]])
 		return result
 
 	def change_rgb_to_hex(self, rgb):
 		"""
 		엑셀의 Cells(1, i).Interior.Color는 hex값을 사용한다
@@ -540,81 +515,103 @@
 					result = self.change_rgb_to_hsl(input_scolor)
 				else: result = input_scolor
 		else:
 			[number_only, color_name, color_step] = self.check_input_scolor(input_scolor)
 
 			if number_only != "":
 				#만약 숫자만 입력을 햇다면, 엑셀 번호로 생각하는것
-				r_no, g_no, b_no = self.color_vars["rgb_56_for_excel"][int(number_only)]
+				r_no, g_no, b_no = self.var["rgb_56_for_excel"][int(number_only)]
 			else:
 				#색을 번호로 변경하는것
 				#print("색이름은 ==> ", color_name)
-				color_name = self.color_vars["check_color_name"][color_name]
+				color_name = self.var["check_color_name"][color_name]
 
 				if color_name =="whi" or color_name =="bla" or color_name =="gra":
 					#만약 색이 흰색, 검정, 회색일경우는 h,s는 0으로 한다
 					l_code_dic = {"bla": 0, "gra": 50, "whi": 100}
 					h_code = 0
 					s_code = 0
 					l_code = int(l_code_dic[color_name]) + int(color_step)
 				elif color_name and color_step == 0:
 					# 기본색 인경우
-					h_code, s_code, l_code = self.color_vars["color_name_eng_vs_hsl_no"][color_name]
+					h_code, s_code, l_code = self.var["color_name_eng_vs_hsl_no"][color_name]
 				else:
 					# 기타 다른 경우
 					#print(color_name)
 					#print(self.basic_12hsl_set)
-					h_code = self.color_vars["color_name_eng_vs_hsl_no"][color_name][0]
+					h_code = self.var["color_name_eng_vs_hsl_no"][color_name][0]
 					s_code = 100
 					l_code = int(color_step)
 
 				if int(l_code) > 100 : l_code = 100
 				if int(l_code) < 0 : l_code = 0
 			#print("[h_code, s_code, l_code] ==> ", h_code, s_code, l_code)
 			result = [h_code, s_code, l_code]
 		return result
 
-	def change_scolor_to_rgb (self, input_scolor):
-		hsl_list = self.change_scolor_to_hsl(input_scolor)
-		result = self.change_hsl_to_rgb(hsl_list)
-		return result
-
 	def change_scolor_to_n_color_set(self, input_scolor, step_no = 10):
 		#하나의 색을 옅은것부터 진한것까지 N개의 rgb값으로 변경하는것
 		hsl_list = self.change_scolor_to_hsl(input_scolor)
 
 		result = []
 		for l in range(0, 110, 10):
 			temp = self.change_hsl_to_rgb([hsl_list[0], 100, l])
 			result.append(temp)
 		return result
 
 
+	def change_scolor_to_rgb (self, input_scolor):
+		hsl_list = self.change_scolor_to_hsl(input_scolor)
+		result = self.change_hsl_to_rgb(hsl_list)
+		return result
+
+	def change_scolor_to_rgb_with_style(self, input_scolor="red45", color_style="파스텔", style_step=5):
+		"""
+		입력된 기본 값을 스타일에 맞도록 바꾸고, 스타일을 강하게 할것인지 아닌것인지를 보는것
+		color_style : pccs의 12가지 사용가능, 숫자로 사용가능, +-의 형태로도 사용가능
+		입력예 : 기본색상, 적용스타일, 변화정도,("red45, 파스텔, 3)
+		변화정도는 5를 기준으로 1~9까지임
+		"""
+		# 넘어온 자료중 color값을 hsl로 변경한다
+		basic_hsl = self.change_scolor_to_hsl(input_scolor)
+		# 스타일을 적용하는것
+		aaa = self.var["color_tone_12_names_vs_no"][color_style]
+		step_2 = self.var["sl_small_step_vs_sl_no"][aaa]
+		# 스타일을 얼마나 강하게 적용할것인가를 나타내는것
+		step_1 = self.var["sl_big_step_vs_sl_no"][str(style_step)]
+
+		h = int(basic_hsl[0])
+		s = int(basic_hsl[1]) + int(step_1[0]) + int(step_2[0])
+		l = int(basic_hsl[2]) + int(step_1[1]) + int(step_2[1])
+
+		changed_rgb = self.change_hsl_to_rgb([h, s, l])
+		return changed_rgb
+
 	def check_change_mode(self, change_mode):
 
 		if type(change_mode) == type([]):
 			result = change_mode
 		elif "+" == str(change_mode)[0]:
 			#현재의 값에서 10만큼 밝아지도록 한다
 			l_value = 10 * len(change_mode)
 			result = [0, 0, l_value]
 		elif "-" == str(change_mode)[0]:
 			#현재의 값에서 10만큼 어두워지도록 한다
 			l_value = -10 * len(change_mode)
 			result = [0, 0, l_value]
-		elif change_mode in self.color_vars["color_tone_12_names_vs_no"].keys():
-			no = self.color_vars["color_tone_12_names_vs_no"][change_mode]
-			result = self.color_vars["sl_big_step_vs_sl_no"][no]
+		elif change_mode in self.var["color_tone_12_names_vs_no"].keys():
+			no = self.var["color_tone_12_names_vs_no"][change_mode]
+			result = self.var["sl_big_step_vs_sl_no"][no]
 		return result
 
 	def check_hsl_value(self, input_color):
 		# 입력으로 들어온 색에 대한 hsl값을 돌려준다
 		try:
-			color_name = self.color_vars["check_color_name"][input_color]
-			result = self.color_vars["color_name_eng_vs_hsl_no"][color_name]
+			color_name = self.var["check_color_name"][input_color]
+			result = self.var["color_name_eng_vs_hsl_no"][color_name]
 		except:
 			pass
 		# 입력된 색이름을 찾을수 없을때
 		return result
 
 	def check_input_color(self, input_value):
 		result = self.change_input_value_to_hsl(input_value)
@@ -642,19 +639,19 @@
 
 		#색을 나타내는 글자를 추출해서,
 		# 기본색이름으로 변경하는 것이다
 		re_com1 = re.compile("[a-zA-Z_가-힣]+")
 		#print("input_scolor", input_scolor)
 		color_str = re_com1.findall(input_scolor)
 		#print("color_str", color_str)
-		#print(self.color_vars["check_color_name"])
+		#print(self.var["check_color_name"])
 
 		if color_str != []:
-			if color_str[0] in self.color_vars["check_color_name"].keys():
-				color_name = self.color_vars["check_color_name"][color_str[0]]
+			if color_str[0] in self.var["check_color_name"].keys():
+				color_name = self.var["check_color_name"][color_str[0]]
 			else:
 				color_name = "not_found_" + str(color_str[0])
 
 		# 새롭게 정의해 보자
 		#숫자로 정도를 표기한것인지를 알기위하여 숫자를 추출한다
 		re_com2 = re.compile("[0-9]+")
 		no_str = re_com2.findall(input_scolor)
@@ -711,22 +708,22 @@
 			if l < 0: l = 0
 
 		result = self.change_hsl_to_rgb([h, s, l])
 		return result
 
 	def control_hsl_value(self, input_hsl, step_no):
 		# +，-로 조정을 하는것이다
-		s, l = self.color_vars["+-_value_vs_sl_no"][step_no]
+		s, l = self.var["+-_value_vs_sl_no"][step_no]
 		result = [input_hsl[0], input_hsl[1] + s, input_hsl[2] + l]
 
 	def control_hsl_with_style(self, basic_hsl, color_style="파스텔", style_step=5):
-		color_style = self.color_vars["check_color_tone"][color_style]
+		color_style = self.var["check_color_tone"][color_style]
 		#print(color_style)
-		step_2 = self.color_vars["color_tone_simple_eng_vs_sl_no"][color_style]
-		step_1 = self.color_vars["sl_small_step_vs_sl_no"][str(str(style_step))]
+		step_2 = self.var["color_tone_simple_eng_vs_sl_no"][color_style]
+		step_1 = self.var["sl_small_step_vs_sl_no"][str(str(style_step))]
 		h = int(basic_hsl[0])
 		s = int(step_1[0]) + int(step_2[0])
 		l = int(step_1[1]) + int(step_2[1])
 
 		changed_rgb = self.change_hsl_to_rgb([h, s, l])
 		return changed_rgb
 
@@ -765,140 +762,137 @@
 		입력예 : 기본색상, 적용스타일, 변화정도,("red45, 파스텔, 3)
 		변화정도는 5를 기준으로 1~9까지임
 		"""
 
 		#넘어온 자료중 color값을 hsl로 변경한다
 		basic_hsl = self.change_scolor_to_hsl(input_scolor)
 		#스타일을 적용하는것
-		step_2 = self.color_vars["sl_small_step_vs_sl_no"][color_style]
+		step_2 = self.var["sl_small_step_vs_sl_no"][color_style]
 		#스타일을 얼마나 강하게 적용할것인가를 나타내는것
-		step_1 = self.color_vars["sl_big_step_vs_sl_no"][str(style_step)]
+		step_1 = self.var["sl_big_step_vs_sl_no"][str(style_step)]
 
 		h = int(basic_hsl[0])
 		s = int(basic_hsl[1]) + int(step_1[1]) + int(step_2[1])
 		l = int(basic_hsl[2]) + int(step_1[2]) + int(step_2[2])
 
 		changed_rgb = self.change_hsl_to_rgb([h,s,l])
 		return changed_rgb
 
 	def data_12_color_name_eng_list(self):
 		"""
 		12가지 영어 색깔이름을 돌려준다
 		['rm', 'bm', 'cya', 'blu', 'gra', '유황', 'red', 'pale_pink', 'mag', 'bc', 'sca', 'yel', 'bla', 'ora', 'bro', 'gy', 'gre', 'scarlet', 'whi', 'gc', 'pin', 'sulphur_yellow']
 		"""
-		result = self.color_vars["color_name_for_basic_12_eng"]
+		result = self.var["color_name_for_basic_12_eng"]
 		return result
 
 	def data_12_color_name_kor_list(self):
 		"""
 		12가지 한글 색깔이름을 돌려준다
 		"""
-		result = self.color_vars["color_name_for_basic_12_kor"]
+		result = self.var["color_name_for_basic_12_kor"]
 		return result
 
 	def data_12_pccs_style_eng_name_list(self):
-		result = self.color_vars["color_tone_eng"]
+		result = self.var["color_tone_eng"]
 		return result
 
 	def data_12_pccs_style_name_list(self):
-		result = self.color_vars["color_tone_kor"]
+		result = self.var["color_tone_kor"]
 
 		return result
 
 	def data_12_rgb_list(self):
-		result = self.color_vars["rgb_for_basic_12"]
+		result = self.var["rgb_for_basic_12"]
 		return result
 
+	def data_46_excel_rgb_list(self):
+		result = self.var["rgb_46_for_excel"]
+		return result
+
+
+
 	def data_all_color_name_list(self):
 		"""
 		모든 색깔의 이름들
 		"""
-		result = list(set(self.color_vars["check_color_name"].values()))
+		result = list(set(self.var["check_color_name"].values()))
 		return result
 
 
 	def data_all_eng_color_name_list(self):
 		"""
 		scolor에서 사용할수있는 모든 영어 색깔의 이름들
 		"""
-		result = self.color_vars["color_name_for_all_eng"]
+		result = self.var["color_name_for_all_eng"]
 		return result
 
 	def data_all_kor_color_name_list(self):
 		"""
 		scolor에서 사용할수있는 모든 한글 색깔의 이름들
 		"""
-		result = self.color_vars["color_name_for_all_kor"]
+		result = self.var["color_name_for_all_kor"]
 		return result
 
 
 	def data_basic_12_hsl_set(self):
 		"""
 		360도의 색을 30도씩 12개로 구분한 hsl분류표
 		"""
-		result = self.color_vars["hsl_no_for_basic_12"]
+		result = self.var["hsl_no_for_basic_12"]
 		return result
 
 	def data_basic_12_pccs_style_eng_name_set(self):
 		"""
 		data로 시작하는 함수는 입력값이 없이 어떤 자료의 형태를 갖고오는 것이다
 		pccs : 일본색체연구서가 빌표한 12가지 색으로 구분한것
 		어떤 입력된 색의 기본적인 PCSS 12색을 돌려준다
 		pccs톤, rgb로 넘어온 색을 pcss톤 12개로 만들어서 돌려준다
 		"""
-		result = self.color_vars["color_tone_eng"]
+		result = self.var["color_tone_eng"]
 		return result
 
 	def data_basic_12_rgb_pccs_style(self, hsl):
 		"""
 		12가지 스타일의 hsl을 돌려주는 것이다
 		"""
 		result = []
-		for one_value in self.color_vars["hsl_no_for_basic_12"]:
+		for one_value in self.var["hsl_no_for_basic_12"]:
 			temp = self.change_hsl_to_rgb([hsl[0], one_value[0], one_value[1]])
 			result.append(temp)
 		return result
 
 	def data_basic_12_rgb_set(self):
 		"""
 		기본적으로 자장된 자료에서 갖고오는 것이다
 		많이 사용하는 다른 색들을 사용하기 위해
 		테두리, 폰트색이나 단색으로 나타낼때 사용하면 좋다
 		"""
-		result = self.color_vars["rgb_for_basic_12"]
+		result = self.var["rgb_for_basic_12"]
 		return result
 
 	def data_basic_12_style_name_set(self):
 		"""
 		스타일에 대한 이름을 갖고오는 것이다
 		"""
-		result = list(self.color_vars["color_tone_12_names_vs_no"].keys())
+		result = list(self.var["color_tone_12_names_vs_no"].keys())
 		return result
 
 	def data_basic_13_color_name_eng_set(self):
 		"""
 		기본 13가지 색의 리스트 : 영어
 		"""
-		result = self.color_vars["color_name_for_basic_12_eng"]
+		result = self.var["color_name_for_basic_12_eng"]
 		return result
 
-	def data_color_tone_kor(self):
-		"""
-		칼라톤에대한 한글이름
-		"""
-		result = self.color_vars["color_tone_kor"]
-		return result
-
-
-
 	def data_basic_13_color_name_kor_set(self):
 		"""
 		기본 13가지 색의 리스트 : 한글
 		"""
-		result = self.color_vars["color_name_for_basic_12_kor"]
+		result = self.var["color_name_for_basic_12_kor"]
 		return result
 
 	def data_basic_36_hsl_set(self):
 		"""
 		기본적인 hsl로된 36색을 갖고온다
 		빨간색을 0으로하여 시작한다
 		결과값 : hsl
@@ -924,42 +918,55 @@
 					result[str(h) + str("_") + str(s) + str("_") + str(l)] = temp
 		return result
 
 	def data_basic_56_excel_rgb_set(self):
 		"""
 		엑셀 기본 rgb 색 : 56색
 		"""
-		result = self.color_vars["rgb_56_for_excel"]
+		result = self.var["rgb_56_for_excel"]
 		return result
 
 	def data_basic_8_pastel_rgb_set(self):
 		"""
 		기본적인
 		자료가 있는 색들의 배경색으로 사용하면 좋은 색들
 		"""
-		color_set = self.color_vars["hsl_no_for_basic_12"][:-4]
+		color_set = self.var["hsl_no_for_basic_12"][:-4]
 		result = []
 		for hsl_value in color_set:
 			rgb = self.control_hsl_with_style(hsl_value, "pastel", 4)
 			result.append(rgb)
 		return result
 
+	def data_basic_color_name_list(self):
+		result = self.var["color_name_for_basic_12_kor"]
+		return result
+
+	def data_basic_color_step(self):
+		result = self.var["basic_color_step"]
+		return result
+
+
+	def data_basic_color_tone_list(self):
+		result = self.var["color_tone_kor"]
+		return result
+
 	def data_basic_faber_rgb_set(self, start_color=11, code=5):
 		"""
 		파버 비덴의의 색체 조화론을 코드로 만든것이다
 		한가지 색에대하 ㄴ조화를 다룬것
 		# White(100-0) - Tone(10-50) - Color(0-0) : 색이 밝고 화사
 		# Color(0-0) - Shade(0-75) - Black(0-100) : 색이 섬세하고 풍부
 		# White(100-0) - GrayGray(25-75) - Black(0-100) : 무채색의 조화
 		# Tint(25-0) - Tone(10-50) - Shade(0-75) 의 조화가 가장 감동적이며 세련됨
 		# White(100-0) - Color(0-0) - Black(0-100) 는 기본적인 구조로 전체적으로 조화로움
 		# Tint(25-0) - Tone(10-50) - Shade(0-75) - Gray(25-75) 의 조화는 빨강, 주황, 노랑, 초록, 파랑, 보라와 모두 조화를 이룬다
 		"""
-		h_list = self.color_vars["hsl_no_for_basic_12"]
-		sl_faber = self.color_vars["sl_no_for_faber_style"]
+		h_list = self.var["hsl_no_for_basic_12"]
+		sl_faber = self.var["sl_no_for_faber_style"]
 
 		h_no = h_list[start_color][0]
 		result = []
 		temp_hsl = sl_faber[code]
 		for one_sl in temp_hsl:
 			rgb = self.change_hsl_to_rgb([h_no, one_sl[0], one_sl[1]])
 			result.append(rgb)
@@ -968,62 +975,71 @@
 	def data_basic_johannes_rgb_set(self, start_color=11, num_color=4, stongness=5):
 		"""
 		요하네스 이텐의 색체 조화론을 코드로 만든것이다
 		"""
 		# start_color : 처음 시작하는 색 번호, 총 색은 12색으로 한다
 		# num_color : 표현할 색의 갯수(2, 3, 4, 6만 사용가능)
 		# stongness : 색의 농도를 나타내는 것, 검정에서 하양까지의 11단계를 나타낸것, 중간이 5이다
-		h_list = self.color_vars["hsl_no_for_basic_12"]
-		sl_list = self.color_vars["sl_no_for_basic_11"]
-		hsl_johannes = self.color_vars["hsl_no_for_johannes_style"]
+		h_list = self.var["hsl_no_for_basic_12"]
+		sl_list = self.var["sl_no_for_basic_11"]
+		hsl_johannes = self.var["hsl_no_for_johannes_style"]
 		color_set = [[], [], [0, 6], [0, 5, 9], [0, 4, 7, 10], [0, 3, 5, 8, 10], [0, 3, 5, 7, 9, 11]]
 
 		h_no = h_list[start_color][0]
 		new_color_set = []
 		for temp in color_set[num_color]:
 			new_color_set.append((temp + int(h_no / 30)) % 12)
 
 		result = []
 		for no in new_color_set:
 			temp_hsl = hsl_johannes[no][stongness]
 			rgb = self.change_hsl_to_rgb(temp_hsl)
 			result.append(rgb)
 		return result
 
+	def data_color_tone_kor(self):
+		"""
+		칼라톤에대한 한글이름
+		"""
+		result = self.var["color_tone_kor"]
+		return result
+
+
+
 	def data_cool_color_name_list(self):
 		"""
 		차가운 색깔의 이름들
 		"""
 		result = ["파랑", "초록", "보라"]
 		return result
 
 	def data_excel_46_rgb_list(self):
-		result = self.color_vars["rgb_46_for_excel"]
+		result = self.var["rgb_46_for_excel"]
 		return result
 
 	def data_excel_56_rgb_list(self):
 		"""
 		엑셀 기본 rgb 색 : 56색
 		"""
-		result = self.color_vars["rgb_56_for_excel"]
+		result = self.var["rgb_56_for_excel"]
 		return result
 
 	def data_worm_color_name_list(self):
 		"""
 		따뜻한 색깔의 이름들
 		"""
 		result = ["빨강", "주황", "노랑"]
 		return result
 
 	def get_rgb_by_excel_color_no(self, input_no):
 		"""
 		엑셀의 기본 번호를 넣으면 rgb값을 돌려주는것
 		엑셀 기본 rgb 색 : 56색
 		"""
-		result = self.color_vars["rgb_56_for_excel"][int(input_no)]
+		result = self.var["rgb_56_for_excel"][int(input_no)]
 		return result
 
 	def get_rgb_list_as_per_input_no (self, input_no=36):
 		"""
 		입력된 숫자만큼, rgt리스트를 갖고오는것
 		기본적인 hsl로된 36색을 갖고온다
 		빨간색을 0으로하여 시작한다
@@ -1052,14 +1068,30 @@
 		return result
 
 	def manual(self):
 		result = 	"""
 			"""
 		return result
 
+	def mix_two_scolors_with_step(self, scolor_1, scolor_2, step=10):
+		# 두가지색을 기준으로 몇단계로 색을 만들어주는 기능
+		# 예를들어, 발강 ~파랑사이의 색을 10단계로 만들어 주는 기능
+		rgb_1 = self.change_scolor_to_rgb(scolor_1)
+		rgb_2 = self.change_scolor_to_rgb(scolor_2)
+		r_step = int((rgb_2[0] - rgb_1[0]) / step)
+		g_step = int((rgb_2[1] - rgb_1[1]) / step)
+		b_step = int((rgb_2[2] - rgb_1[2]) / step)
+		result = [rgb_1, ]
+		for no in range(1, step - 1):
+			new_r = int(rgb_1[0] + r_step * no)
+			new_g = int(rgb_1[1] + g_step * no)
+			new_b = int(rgb_1[2] + b_step * no)
+			result.append([new_r, new_g, new_b])
+			result.append(rgb_2)
+		return result
 	def move_hsl_to_bright_style(self, input_hsl, strong_level=0.5):
 		"""
 		입력받은 hsl값을 명도가 높은 쪽으로 이동시키는것
 		bright = [100,100], sharp = [50,100], graish = [100,0], dark = [0,0], black = [50, 0]
 		"""
 		h, s, l = input_hsl
 		style = bright = [100,100]
@@ -1129,25 +1161,8 @@
 
 		changed_s = s + delta_s
 		changed_l = l + delta_l
 		return [h, changed_s, changed_l]
 	def terms(self):
 		result = 	"""
 			"""
-		return result
-
-	def mix_two_scolors_with_step(self, scolor_1, scolor_2, step=10):
-		# 두가지색을 기준으로 몇단계로 색을 만들어주는 기능
-		# 예를들어, 발강 ~파랑사이의 색을 10단계로 만들어 주는 기능
-		rgb_1 = self.change_scolor_to_rgb(scolor_1)
-		rgb_2 = self.change_scolor_to_rgb(scolor_2)
-		r_step = int((rgb_2[0] - rgb_1[0]) / step)
-		g_step = int((rgb_2[1] - rgb_1[1]) / step)
-		b_step = int((rgb_2[2] - rgb_1[2]) / step)
-		result = [rgb_1, ]
-		for no in range(1, step - 1):
-			new_r = int(rgb_1[0] + r_step * no)
-			new_g = int(rgb_1[1] + g_step * no)
-			new_b = int(rgb_1[2] + b_step * no)
-			result.append([new_r, new_g, new_b])
-			result.append(rgb_2)
 		return result
```

### Comparing `xython-1.3.0/src/xython/youtil.py` & `xython-1.4.0/src/xython/youtil.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # -*- coding: utf-8 -*-
 import shutil#내장모듈
 import pickle #내장모듈
 import inspect #내장모듈
 import re #내장모듈
 import os #내장모듈
 import random #내장모듈
+import collections #내장모듈
 from difflib import SequenceMatcher #내장모듈
 
-import basic_data  # halmoney 모듈
-import pynal  # halmoney 모듈
-import pyclick  # halmoney 모듈
+import basic_data  # xython 모듈
 
-class youtil(pynal.pynal, pyclick.pyclick):
+
+class youtil():
 	"""
 	여러가지 사무용에 사용할 만한 메소드들을 만들어 놓은것이며,
 	좀더 특이한 것은 youtil2로 만들어서 사용할 예정입니다 
 	"""
 	def __init__(self):
-		super().__init__()
 		self.base_data = basic_data.basic_data()
 		self.var = self.base_data.vars
-		#공통으로 사용할 변수들을 설정하는 것
+		self.var_common={} #공통으로 사용할 변수들을 설정하는 것
 
 	def append_input_value_at_each_list1d_in_list2d(self, input_list2d, input_value):
 		"""
 		같은 항목으로 되어있는 자료를 제일 처음의 자료를 기준으로 합치는것
 		2차원 리스트의 모든 자료끝에 값 추가하기
 		"""
 		result = []
@@ -137,20 +136,20 @@
 		초성 19자 : ㄱ,ㄲ,ㄴ,ㄷ,ㄸ,ㄹ,ㅁ,ㅂ,ㅃ,ㅅ,ㅆ,ㅇ,ㅈ,ㅉ,ㅊ,ㅋ,ㅌ,ㅍ,ㅎ
 		중성 21자 : ㅏ,ㅐ,ㅑ,ㅒ,ㅓ,ㅔ,ㅕ,ㅖ,ㅗ,ㅘ,ㅙ,ㅚ,ㅛ,ㅜ,ㅝ,ㅞ,ㅟ,ㅠ,ㅡ,ㅢ,ㅣ
 		종성 28자 : (없음),ㄱ,ㄲ,ㄳ,ㄴ,ㄵ,ㄶ,ㄷ,ㄹ,ㄺ,ㄻ,ㄼ,ㄽ,ㄾ,ㄿ,ㅀ,ㅁ,ㅂ,ㅄ,ㅅ,ㅆ,ㅇ,ㅈ,ㅊ,ㅋ,ㅌ,ㅍ,ㅎ
 		"""
 		result = []
 		for one_jamo in input_jamo_list:
 			#유니코드의 순서대로 번호를 붙인것에서 순서를 읽어온다
-			chosung_no = self.var["first_letter_no"][one_jamo[0]]  # 초성
-			joongsung_no = self.var["second_letter_no"][one_jamo[1]]  # 중성
+			chosung_no = self.var["list_자음_19"][one_jamo[0]]  # 초성
+			joongsung_no = self.var["list_모음_21"][one_jamo[1]]  # 중성
 			try:
-				jongsung_no = self.var["third_letter_no"][one_jamo[2]]  # 종성
+				jongsung_no = self.var["list_받침_28"][one_jamo[2]]  # 종성
 			except:
-				jongsung_no = self.var["third_letter_no"][""]  # 종성
+				jongsung_no = self.var["list_받침_28"][""]  # 종성
 
 			#한글이 시작되는 번호 44032번째부터 몇번째인지를 계산하는것
 			unicode_no = chosung_no*21*28 + joongsung_no*28 + jongsung_no + 44032
 			#print(one_jamo, " ==> unicode_no ==> ", unicode_no)
 			result.append(chr(unicode_no))
 		return result
 
@@ -539,15 +538,15 @@
 		"""
 		연속된 같은 자료만 지우는 것
 		"""
 		result = []
 		for no in range(len(input_list)-1):
 			if input_list[no] == input_list[no+1]:
 				pass
-				#excel.write_value_in_cell("", [no+3, "ae"], "")
+				#self.write_value_in_cell("", [no+3, "ae"], "")
 			else:
 				result.append(input_list[no])
 		return result
 
 	def delete_empty_value_in_list(self, input_list, condition=["", None, [], ()]):
 		"""
 		넘어온 리스트 형태의 자료중 조건에 맞는것이 있으면 제거하는 것
@@ -1062,36 +1061,14 @@
 	def sort_list2d(self, input_list2d):
 		"""
 		2차원 리스트를 정렬하는 것
 		"""
 		result=self.sort_list2d_by_index(input_list2d, index_no=0)
 		return result
 
-	def sort_list2d_by_index(self, input_list2d, index_no=0):
-		"""
-		입력 :  리스트자료
-		리스트자료를 몇번째 순서를 기준으로 정렬하는것
-		숫자와 문자가 같이 섞여 있어도, 정렬이 가능
-		aa = [[111, 'abc'], [222, 222],['333', 333], ['777', 'sjpark'], ['aaa', 123],['zzz', 'sang'], ['jjj', 987], ['ppp', 'park']]
-		value=sort_list(리스트자료, 정렬기준번호)
-		"""
-
-		str_temp = []
-		int_temp = []
-		for one in input_list2d:
-			if type(one[index_no]) == type("str"):
-				str_temp.append(one)
-			else:
-				int_temp.append(one)
-
-		result_int = sorted(int_temp, key=lambda x: x[index_no])
-		result_str = sorted(str_temp, key=lambda x: x[index_no])
-		result = result_int + result_str
-
-		return result
 
 	def sort_mixed_list1d(self, input_list1d):
 		"""
 		1, 2차원의 자료가 섞여서 저장된 자료를 정렬하는 것
 		"""
 		int_list = sorted([i for i in input_list1d if type(i) is float or type(i) is int])
 		str_list = sorted([i for i in input_list1d if type(i) is str])
@@ -1301,21 +1278,43 @@
 			new_no_2 = (int(one_byte_data[1]) - 128) * 64
 			new_no_3 = (int(one_byte_data[2]) - 128)
 			#유니코드의 번호로 바꾼다
 			#한글의 경우는 44032번째부터 순서대로 표시되어있다
 			value = new_no_1 + new_no_2 + new_no_3 - 3072
 
 			#print("value", value)
-			chosung = self.var["first_letter"][divmod(value, 588)[0]]  # 초성
-			joongsung = self.var["second_letter"][divmod(divmod(value, 588)[1], 28)[0]]  # 중성
-			jongsung = self.var["third_letter"][divmod(divmod(value, 588)[1], 28)[1]]  # 종성
+			chosung = self.var["list_자음_19"][divmod(value, 588)[0]]  # 초성
+			joongsung = self.var["list_모음_21"][divmod(divmod(value, 588)[1], 28)[0]]  # 중성
+			jongsung = self.var["list_받침_28"][divmod(divmod(value, 588)[1], 28)[1]]  # 종성
 			result.append(([chosung, joongsung, jongsung]))
 			#print(divmod(value, 588), divmod(divmod(value, 588)[1], 28))
 		return result
 
+
+	def split_hangul_to_jamo(self, one_text):
+		"""
+		한글자의 한글을 자음과 모음으로 구분해 주는것
+		"""
+		one_byte_data = one_text.encode("utf-8")
+
+		new_no_1 = (int(one_byte_data[0]) - 234) * 64 * 64
+		new_no_2 = (int(one_byte_data[1]) - 128) * 64
+		new_no_3 = (int(one_byte_data[2]) - 128)
+
+		value = new_no_1 + new_no_2 + new_no_3 - 3072
+
+		temp_num_1 = divmod(value, 588)  # 초성이 몇번째 자리인지를 알아내는것
+		temp_num_2 = divmod(divmod(value, 588)[1], 28)  # 중성과 종성의 자릿수를 알아내는것것
+
+		chosung = self.var["list_자음_19"][divmod(value, 588)[0]]  # 초성
+		joongsung = self.var["list_모음_21"][divmod(divmod(value, 588)[1], 28)[0]]  # 중성
+		jongsung = self.var["list_받침_28"][divmod(divmod(value, 588)[1], 28)[1]]  # 종성
+
+		return [chosung, joongsung, jongsung]
+
 	def split_list1d_by_group_no(self, input_list1d, step_no):
 		"""
 		12개의 리스트를
 		입력 : [ [1,2,3,4,5,6,7,8,9,10,11,12], 4]를 받으면
 				총 4개의 묶읆으로 순서를 섞어서 만들어 주는것
 			   [[1,5,9],  [2,6,10],  [3,7,11],  [4,8,12]] 로 만들어 주는것
 		"""
@@ -1670,15 +1669,15 @@
 	def float_range(self, start, end, step):
 		# 실수형으로 가능한 range 형태
 		value = start
 		while value <= end:
 			yield value
 			value = step + value
 
-	def sample_make_name(self, input_no=5):
+	def data_make_sample_name(self, input_no=5):
 		# 입력한 갯수만큼 이름의 갯수를 만들어 주는것
 		sung = "김이박최정강조윤장"
 		name = "가나다라마바사아자차카"
 		last = "진원일이삼사오구원송국한"
 		if input_no > len(sung) * len(name) * len(last) / 2:
 			result = []
 			pass
@@ -1692,8 +1691,622 @@
 				new_name = one_sung + one_name + one_last
 				total_name.add(new_name)
 				num = num + 1
 				if len(total_name) == input_no:
 					print(input_no, num)
 					break
 			result = list(total_name)
+		return result
+
+
+
+	def get_moum_xy_list(self, size=[1, 2], input_data="ㅏ"):
+		# 모음을 엑셀에 나타내기 위한 좌표를 주는 것이다
+		x, y = size
+		# x, y는 글자의 크기
+		mo_01 = [["ㅏ"], [1, 0.6 * y, x, 0.6 * y],
+				 [0.4 * x, 0.6 * y, 0.4 * x, 0.8 * y]]
+		mo_02 = [["ㅑ"], [1, 0.6 * y, x, 0.6 * y],
+				 [0.4 * x, 0.6 * y, 0.4 * x, 0.8 * y],
+				 [0.6 * x, 0.6 * y, 0.6 * x, 0.8 * y]]
+		mo_03 = [["ㅓ"], [1, 0.6 * y, x, 0.6 * y],
+				 [0.4 * x, 0.4 * y, 0.4 * x, 0.6 * y]]
+		mo_04 = [["ㅕ"], [1, 0.6 * y, x, 0.6 * y],
+				 [0.4 * x, 0.4 * y, 0.4 * x, 0.6 * y],
+				 [0.6 * x, 0.4 * y, 0.6 * x, 0.6 * y]]
+		mo_10 = [["ㅣ"], [1, 0.6 * y, x, 0.6 * y]]
+		mo_05 = [["ㅗ"], [x, 1, x, y],
+				 [x, 0.5 * y, 0.8 * x, 0.5 * y]]
+		mo_06 = [["ㅛ"], [x, 1, x, y],
+				 [x, 0.3 * y, 0.8 * x, 0.3 * y],
+				 [x, 0.7 * y, 0.8 * x, 0.7 * y]]
+		mo_07 = [["ㅜ"], [1, 1, 1, y],
+				 [1, 0.5 * y, 0.5 * x, 0.5 * y]]
+		mo_08 = [["ㅠ"], [1, 1, 1, y],
+				 [1, 0.3 * y, 0.8 * x, 0.3 * y],
+				 [1, 0.7 * y, 0.8 * x, 0.7 * y]]
+		mo_09 = [["ㅡ"], [0.5 * x, 1, 0.5 * x, y]]
+
+		mo_21 = [["ㅐ"], [1, 0.6 * y, x, 0.6 * y],
+				 [1, 0.8 * y, x, 0.8 * y],
+				 [0.4 * x, 0.6 * y, 0.4 * x, 0.8 * y]]
+		mo_22 = [["ㅒ"], [1, 0.6 * y, x, 0.6 * y],
+				 [1, 0.8 * y, x, 0.8 * y],
+				 [0.4 * x, 0.6 * y, 0.4 * x, 0.6 * y],
+				 [0.6 * x, 0.8 * y, 0.6 * x, 0.8 * y]]
+		mo_23 = [["ㅔ"], [1, 0.6 * y, x, 0.6 * y],
+				 [1, 0.8 * y, x, 0.8 * y],
+				 [0.4 * x, 0.4 * y, 0.4 * x, 0.6 * y]]
+		mo_24 = [["ㅖ"], [1, 0.6 * y, x, 0.6 * y],
+				 [1, 0.8 * y, x, 0.8 * y],
+				 [0.4 * x, 0.4 * y, 0.4 * x, 0.6 * y],
+				 [0.6 * x, 0.4 * y, 0.6 * x, 0.6 * y]]
+
+		jamo2_dic = {
+			"ㅏ": mo_01, "ㅑ": mo_02, "ㅓ": mo_03, "ㅕ": mo_04, "ㅗ": mo_05,
+			"ㅛ": mo_06, "ㅜ": mo_07, "ㅠ": mo_08, "ㅡ": mo_09, "ㅣ": mo_10,
+			"ㅐ": mo_21, "ㅒ": mo_22, "ㅔ": mo_23, "ㅖ": mo_24,
+		}
+		result = jamo2_dic[input_data]
+		return result
+
+	def get_jaum_xy_list(self, size=[1, 2], input_data="ㄱ"):
+		x, y = size
+		# x, y는 글자의 크기
+		ja_01 = [["ㄱ"], [1, 1, 1, y], [1, y, x, y]]
+		ja_02 = [["ㄴ"], [1, 1, x, 1], [x, 1, x, y]]
+		ja_03 = [["ㄷ"], [1, y, 1, 1], [1, 1, x, 1], [x, 1, x, y]]
+		ja_04 = [["ㄹ"], [1, 1, 1, y], [1, y, 0.5 * x, y], [0.5 * x, y, 0.5 * x, 1], [0.5 * x, 1, x, 1], [x, 1, x, y]]
+		ja_05 = [["ㅁ"], [1, 1, 1, y], [1, y, x, y], [x, y, x, 1], [x, 1, 1, 1]]
+		ja_06 = [["ㅂ"], [1, 1, x, 1], [x, 1, x, y], [x, y, 1, y], [0.5 * x, 1, 0.5 * x, y]]
+		ja_07 = [["ㅅ"], [1, 0.5 * y, 0.3 * x, 0.5 * y], [0.3 * x, 0.5 * y, x, 1], [0.3 * x, 0.5 * y, x, y]]
+		ja_08 = [["ㅇ"], [0.8 * x, 0.2 * y, 0.8 * x, 0.8 * y], [0.8 * x, 0.8 * y, 0.6 * x, y, ""],
+				 [0.6 * x, y, 0.2 * x, y], [0.2 * x, y, 1, 0.8 * y, "/"], [1, 0.8 * y, 1, 0.2 * y],
+				 [1, 0.2 * y, 0.2 * x, 1, ""], [0.2 * x, 1, 0.6 * x, 1], [0.6 * x, 1, 0.8 * x, 0.2 * y, "/"]]
+		ja_09 = [["ㅈ"], [1, 1, 1, y], [1, 0.5 * y, 0.5 * x, 0.5 * y], [0.5 * x, 0.5 * y, x, 1, "/"],
+				 [0.5 * x, 0.5 * y, x, y, ""]]
+		ja_10 = [["ㅊ"], [0.2 * x, 0.5 * y, 1, 0.5 * y], [0.2 * x, 1, 0.2 * x, y], [0.2 * x, 0.5 * y, 0.4 * x, 0.5 * y],
+				 [1, 0.5 * y, 0.5 * x, 0.5 * y], [0.5 * x, 0.5 * y, x, 1], [0.5 * x, 0.5 * y, x, y, ""]]
+		ja_11 = [["ㅋ"], [1, 1, 1, y], [1, y, x, y], [0.5 * x, 1, 0.5 * x, y]]
+		ja_12 = [["ㅌ"], [1, y, 1, 1], [1, 1, x, 1], [x, 1, x, y], [0.5 * x, 1, 0.5 * x, y]]
+		ja_13 = [["ㅍ"], [1, 1, 1, y], [x, 1, x, y], [1, 0.2 * y, x, 0.2 * y], [1, 0.8 * y, x, 0.8 * y]]
+		ja_14 = [["ㅎ"], [1, 0.5 * y, 0.2 * x, 0.5 * y], [0.2 * x, 1, 0.2 * x, y], [0.4 * x, 0.3 * y, 0.4 * x, 0.8 * y],
+				 [0.4 * x, 0.8 * y, 0.6 * x, y], [0.6 * x, y, 0.8 * x, y], [0.8 * x, y, x, 0.8 * y],
+				 [x, 0.8 * y, x, 0.3 * y], [x, 0.3 * y, 0.8 * x, 1], [0.8 * x, 1, 0.6 * x, 1],
+				 [0.6 * x, 1, 0.4 * x, 0.3 * y]]
+		ja_31 = [["ㄲ"], [1, 1, 1, 0.4 * y], [1, 0.4 * y, x, 0.4 * y], [1, 0.7 * y, 1, y], [1, y, x, y], ]
+		ja_32 = [["ㄸ"], [1, 1, 1, 0.4 * y], [1, 1, x, 1], [x, 1, x, 0.4 * y], [1, 0.7 * y, 1, y],
+				 [1, 0.7 * y, x, 0.7 * y], [x, 0.7 * y, x, y], ]
+		ja_33 = [["ㅃ"], [1, 1, x, 1], [x, 1, x, 0.4 * y], [x, 0.4 * y, 1, 0.4 * y], [0.5 * x, 1, 0.5 * x, 0.4 * y],
+				 [1, 0.7 * y, x, 0.7 * y], [x, 0.7 * y, x, y], [x, y, 1, y], [0.5 * x, 0.7 * y, 0.5 * x, y], ]
+		ja_34 = [["ㅆ"], [1, 0.3 * y, 0.4 * x, 0.3 * y], [0.4 * x, 0.3 * y, x, 1], [0.4 * x, 0.3 * y, x, 0.5 * y],
+				 [1, 0.8 * y, 0.4 * x, 0.8 * y], [0.4 * x, 0.8 * y, x, 0.6 * y], [0.4 * x, 0.8 * y, x, y], ]
+		ja_35 = [["ㅉ"], [1, 1, 1, 0.5 * y], [1, 0.3 * y, 0.4 * x, 0.3 * y], [0.4 * x, 0.3 * y, x, 1],
+				 [0.4 * x, 0.3 * y, x, 0.5 * y], [1, 0.6 * y, 1, y], [1, 0.8 * y, 0.4 * x, 0.8 * y],
+				 [0.4 * x, 0.8 * y, x, 0.6 * y], [0.4 * x, 0.8 * y, x, y], ]
+		ja_36 = [["ㄳ"], [1, 1, 1, 0.4 * y], [1, 0.4 * y, x, 0.4 * y], [1, 0.8 * y, 0.4 * x, 0.8 * y],
+				 [0.4 * x, 0.8 * y, x, 0.6 * y], [0.4 * x, 0.8 * y, x, y], ]
+		ja_37 = [["ㄵ"], [1, 1, x, 1], [x, 1, x, 0.4 * y], [1, 0.6 * y, 1, y], [1, 0.8 * y, 0.4 * x, 0.8 * y],
+				 [0.4 * x, 0.8 * y, x, 0.6 * y], [0.4 * x, 0.8 * y, x, y], ]
+		ja_38 = [["ㄶ"], [1, 1, x, 1], [x, 1, x, 0.4 * y], [0.1 * x, 0.8 * y, 1, 0.8 * y],
+				 [0.2 * x, 0.6 * y, 0.2 * x, y], [0.4 * x, 0.7 * y, 0.4 * x, 0.9 * y], [0.4 * x, 0.9 * y, 0.6 * x, y],
+				 [0.6 * x, y, x, 0.9 * y], [x, 0.9 * y, x, 0.7 * y], [x, 0.7 * y, 0.8 * x, 0.6 * y],
+				 [0.8 * x, 0.6 * y, 0.6 * x, 0.6 * y], [0.6 * x, 0.6 * y, 0.4 * x, 0.7 * y]]
+		ja_39 = [["ㄺ"], [1, 1, 1, 0.4 * y], [1, 0.4 * y, 0.5 * x, 0.4 * y], [0.5 * x, 0.4 * y, 0.5 * x, 1],
+				 [0.5 * x, 1, x, 1], [x, 1, x, 0.4 * y], [1, 0.7 * y, 1, y], [1, y, x, y], ]
+		ja_40 = [["ㄻ"], [1, 1, 1, 0.4 * y], [1, 0.4 * y, 0.5 * x, 0.4 * y], [0.5 * x, 0.4 * y, 0.5 * x, 1],
+				 [0.5 * x, 1, x, 1], [x, 1, x, 0.4 * y], [1, 0.7 * y, 1, y], [1, y, x, y], [x, y, x, 0.7 * y],
+				 [x, 0.7 * y, 1, 0.7 * y], ]
+		ja_41 = [["ㄼ"], [1, 1, 1, 0.4 * y], [1, 0.4 * y, 0.5 * x, 0.4 * y], [0.5 * x, 0.4 * y, 0.5 * x, 1],
+				 [0.5 * x, 1, x, 1], [x, 1, x, 0.4 * y], [1, 0.7 * y, x, 0.7 * y], [x, 0.7 * y, x, y], [x, y, 1, y],
+				 [0.5 * x, 0.7 * y, 0.5 * x, y], ]
+		ja_42 = [["ㄽ"], [1, 1, 1, 0.4 * y], [1, 0.4 * y, 0.5 * x, 0.4 * y], [0.5 * x, 0.4 * y, 0.5 * x, 1],
+				 [0.5 * x, 1, x, 1], [x, 1, x, 0.4 * y], [1, 0.8 * y, 0.4 * x, 0.8 * y], [0.4 * x, 0.8 * y, x, 0.6 * y],
+				 [0.4 * x, 0.8 * y, x, y], ]
+		ja_43 = [["ㄾ"], [1, 1, 1, 0.4 * y], [1, 0.4 * y, 0.5 * x, 0.4 * y], [0.5 * x, 0.4 * y, 0.5 * x, 1],
+				 [0.5 * x, 1, x, 1], [x, 1, x, 0.4 * y], [1, 0.7 * y, 1, y], [1, 0.7 * y, x, 0.7 * y],
+				 [x, 0.7 * y, x, y], [0.5 * x, 0.7 * y, 0.5 * x, y], ]
+		ja_44 = [["ㄿ"], [1, 1, 1, 0.4 * y], [1, 0.4 * y, 0.5 * x, 0.4 * y], [0.5 * x, 0.4 * y, 0.5 * x, 1],
+				 [0.5 * x, 1, x, 1], [x, 1, x, 0.4 * y], [1, 0.6 * y, 1, y], [x, 0.6 * y, x, y],
+				 [1, 0.7 * y, x, 0.7 * y], [1, 0.9 * y, x, 0.9 * y], ]
+		ja_45 = [["ㅀ"], [1, 1, 1, 0.4 * y], [1, 0.4 * y, 0.5 * x, 0.4 * y], [0.5 * x, 0.4 * y, 0.5 * x, 1],
+				 [0.5 * x, 1, x, 1], [x, 1, x, 0.4 * y], [0.1 * x, 0.8 * y, 1, 0.8 * y], [0.2 * x, 0.6 * y, 0.2 * x, y],
+				 [0.4 * x, 0.7 * y, 0.4 * x, 0.9 * y], [0.4 * x, 0.9 * y, 0.6 * x, y], [0.6 * x, y, x, 0.9 * y],
+				 [x, 0.9 * y, x, 0.7 * y], [x, 0.7 * y, 0.8 * x, 0.6 * y], [0.8 * x, 0.6 * y, 0.6 * x, 0.6 * y],
+				 [0.6 * x, 0.6 * y, 0.4 * x, 0.7 * y]]
+		ja_46 = [["ㅄ"], [1, 1, x, 1], [x, 1, x, 0.4 * y], [x, 0.4 * y, 1, 0.4 * y], [0.5 * x, 1, 0.5 * x, 0.4 * y],
+				 [1, 0.8 * y, 0.4 * x, 0.8 * y], [0.4 * x, 0.8 * y, x, 0.6 * y], [0.4 * x, 0.8 * y, x, y], ]
+
+		jamo1_dic = {"ㄱ": ja_01, "ㄴ": ja_02, "ㄷ": ja_03, "ㄹ": ja_04, "ㅁ": ja_05,
+					 "ㅂ": ja_06, "ㅅ": ja_07, "ㅇ": ja_08, "ㅈ": ja_09, "ㅊ": ja_10,
+					 "ㅋ": ja_11, "ㅌ": ja_12, "ㅍ": ja_13, "ㅎ": ja_14,
+					 "ㄲ": ja_31, "ㄸ": ja_32, "ㅃ": ja_33, "ㅆ": ja_34, "ㅉ": ja_35,
+					 "ㄳ": ja_36, "ㄵ": ja_37, "ㄶ": ja_38, "ㄺ": ja_39, "ㄻ": ja_40,
+					 "ㄼ": ja_41, "ㄽ": ja_42, "ㄾ": ja_43, "ㄿ": ja_44, "ㅀ": ja_45, "ㅄ": ja_46,
+					 }
+
+		result = jamo1_dic[input_data]
+		return result
+
+	def split_double_moum(self, double_moum):
+		result = self.split_double_moum(double_moum)
+		return result
+
+	def split_double_moum_to_two_simple_moum(self, double_moum):
+		# 이중모음을 단모음으로 바꿔주는것
+		mo2_dic = {"ㅘ": ["ㅗ", "ㅏ"], "ㅙ": ["ㅗ", "ㅐ"], "ㅚ": ["ㅗ", "ㅣ"], "ㅝ": ["ㅜ", "ㅓ"], "ㅞ": ["ㅜ", "ㅔ"], "ㅟ": ["ㅜ", "ㅣ"],
+				   "ㅢ": ["ㅡ", "ㅣ"], }
+		result = mo2_dic[double_moum]
+		return result
+
+
+	def write_hangul_cjj(self, letters="박상진", canvas_size=[50, 50], stary_xy=[1, 1]):
+		# 입력받은 한글을 크기가 50 x 50의 엑셀 시트에 글씨를 색칠하여 나타내는 것이다
+
+		# 기본 설정부분
+		size_x = canvas_size[0]
+		size_y = canvas_size[1]
+		# 문자 하나의 기본크기
+		# 기본문자는 10을 기준으로 만들었으며, 이것을 얼마만큼 크게 만들것인지 한글자의 배수를 정하는것
+		h_mm = int(canvas_size[0] / 10)
+		w_mm = int(canvas_size[1] / 10)
+		# 시작위치
+		h_start = stary_xy[0]
+		w_start = stary_xy[1]
+
+		check_han = re.compile("[ㄱ-ㅎ|ㅏ-ㅣ|가-힣]")
+		for one_char in letters:
+			# 한글을 초성, 중성, 종성으로 나누는 것이다
+			if check_han.match(one_char):
+				jamo123 = self.split_hangul_to_jamo(one_char)
+				if jamo123[0][2] == "":
+					# 가, 나, 다
+					if jamo123[0][1] in ["ㅏ", "ㅐ", "ㅑ", "ㅒ", "ㅓ", "ㅔ", "ㅕ", "ㅖ", "ㅣ"]:
+						# 기본설정은 시작점은 [1,1]이며, 캔버스의 크기는 [50, 50]인것이다
+
+						start_xy = [1, 1]
+						size = [10, 5]  # 위에서 배수를 5,5를 기본으로 해서 50x50되는 것이다
+						# 자음의 시작점은 1,1이며, 크기는 50 x 25의 사이즈의 자음을 만드는 것이다
+						self.draw_jaum_color(jamo123[0][0],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						# 모음의 시작점은 자음의 끝점에서 5를 이동한 1,30이며, 크기는 자음보다 가로의 크기를 좀 줄인
+						# 50 x 20의 사이즈의 자음을 만드는 것이다
+
+						start_xy = [1, 7]
+						size = [10, 4]
+						self.draw_moum_color(jamo123[0][1],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+
+					# 구, 누, 루
+					if jamo123[0][1] in ["ㅗ", "ㅛ", "ㅜ", "ㅡ"]:
+						start_xy = [1, 1]
+						size = [4, 10]
+						self.draw_jaum_color(jamo123[0][0],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [6, 1]
+						size = [5, 10]
+						self.draw_moum_color(jamo123[0][1],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+
+					# 와, 왜, 궈
+					if jamo123[0][1] in ["ㅘ", "ㅙ", "ㅚ", "ㅝ", "ㅞ", "ㅟ", "ㅢ"]:
+						# lists = self.div_mo2_mo1(jamo123[0][1])
+
+						start_xy = [1, 1]
+						size = [10, 5]
+						self.draw_jaum_color(jamo123[0][0],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [8, 1]
+						size = [3, 8]
+						self.draw_moum_color(jamo123[0][1],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [1, 8]
+						size = [6, 3]
+						self.draw_moum_color(jamo123[0][1],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+
+				if jamo123[0][2] != "":
+					# 왕, 웍, 윔
+					if jamo123[0][1] in ["ㅘ", "ㅙ", "ㅚ", "ㅝ", "ㅞ", "ㅟ", "ㅢ"]:
+						hangul_type = "23자음+1332-2중모음+24자음"
+						# lists = div_mo2_mo1(jamo123[0][1])
+
+						start_xy = [1, 1]
+						size = [4, 5]
+						self.draw_jaum_color(jamo123[0][0],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [4, 1]
+						size = [3, 7]
+						self.draw_moum_color(jamo123[0][1],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [1, 7]
+						size = [6, 3]
+						self.draw_moum_color(jamo123[0][1],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [8, 1]
+						size = [3, 6]
+						self.draw_jaum_color(jamo123[0][0],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+
+					# 앙, 양, 건
+					if jamo123[0][1] in ["ㅏ", "ㅐ", "ㅑ", "ㅒ", "ㅓ", "ㅔ", "ㅕ", "ㅖ", "ㅣ"]:
+						start_xy = [1, 1]
+						size = [3, 5]
+						self.draw_jaum_color(jamo123[0][0],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [1, 6]
+						size = [5, 4]
+						self.draw_moum_color(jamo123[0][1],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [7, 2]
+						size = [3, 6]
+						self.draw_jaum_color(jamo123[0][0],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+
+					# 곡, 는
+					if jamo123[0][1] in ["ㅗ", "ㅛ", "ㅜ", "ㅡ"]:
+						start_xy = [1, 1]
+						size = [3, 10]
+						self.draw_jaum_color(jamo123[0][0],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [4, 1]
+						size = [3, 10]
+						self.draw_moum_color(jamo123[0][1],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+						start_xy = [8, 1]
+						size = [3, 10]
+						self.draw_jaum_color(jamo123[0][0],
+											 [h_start + h_mm * (start_xy[0] - 1), w_start + w_mm * (start_xy[1] - 1)],
+											 [h_mm * size[0], w_mm * size[1]])
+
+
+
+#=============================================================================================
+
+	def insert_list2d_blank_by_index(self, input_list2d, no_list):
+		# 입력형태 : 2차원리스트, [2,5,7]
+		no_list.sort()
+		no_list.reverse()
+		for one in no_list:
+			for x in range(len(input_list2d)):
+				input_list2d[x].insert(int(one), "")
+		return input_list2d
+
+
+	def move_list2d_by_index_old(self, input_list2d, input_no_list):
+		# 입력형태 : 2차원리스트, [[옮길것, 옮기고싶은자리].....]
+		input_no_list.sort()
+		input_no_list.reverse()
+		for before, after in input_no_list:
+			for no in range(len(input_list2d)):
+				if before < after:
+					after = after - 1
+				value = input_list2d[no][before]
+				del input_list2d[no][before]
+				input_list2d[no].insert(int(after), value)
+		return input_list2d
+
+
+	def move_list2d_by_index(self, input_list2d, input_no_list):
+		# 입력형태 : 2차원리스트, [[옮길것, 옮기고싶은자리].....]
+
+		ori_no_dic = {}
+		for one in range(len(input_list2d[0])):
+			ori_no_dic[one] = one
+		for before, after in input_no_list:
+			new_before = ori_no_dic[before]
+			new_after = ori_no_dic[after]
+
+			for no in range(len(input_list2d)):
+				if new_before < new_after:
+					new_after = after - 1
+				value = input_list2d[no][new_before]
+				del input_list2d[no][new_before]
+				input_list2d[no].insert(int(new_after), value)
+		return input_list2d
+
+
+	def make_html_table(self, table_title_list, table_value_list):
+		body_top = """
+		수고합니다<br>
+		<br>
+		구매 요청건에 대하여 아래와 같이 TBE요청합니다"<br>
+		<br>
+		"""
+
+		body_tail = """
+		<br>
+		-----------------------------------------------------------------------------------<br>
+		롯데정밀화학 / 구매2팀 / 박상진 수석<br>
+		06181 서울 강남구 테헤란로 534 글라스타워 27층<br>
+		SangJin Park / Procurement 2 Team / Senior Manager<br>
+		LOTTE Fine Chemical Co., LTD<br>
+		27F, Glasstower Bldg., / 534, Teheran-ro, Gangnam-gu, Seoul, 06181, Korea<br>
+		Tel	 : 82-2-6974-4539			   C.P	: 010-3334-0053<br>
+		e-mail : sjp@lotte.net<br>
+		<br>
+		"""
+
+		table_style = """
+		<html>
+		<style>
+		body {
+			  font-family:'Malgun Gothic';
+			  font-size:10pt;
+			}
+		 table {
+			width: 70%;
+			padding: 11px;
+			font-family:'Malgun Gothic';
+			font-size:10pt;
+		  }
+		  tr, td {
+			border-bottom: 1px solid #444444;
+			padding: 3px;
+			text-align: center;
+		  }
+		  tr, th {
+			padding: 13px;
+			background-color: #bbdefb;
+		  }
+		  td {
+			background-color: #e3f2fd;
+		  }
+			</style>
+			<body>"""
+
+		temp = table_style + body_top + "<table>"
+
+		temp = temp + "<tr>"
+		for x in range(len(table_title_list)):
+			temp = temp + "<th>" + str(table_title_list[x]) + "</th>"
+		temp = temp + "</tr>"
+
+		for x in range(len(table_value_list)):
+			temp = temp + "<tr>"
+			for y in range(len(table_value_list[0])):
+				temp = temp + "<td>" + str(table_value_list[x][y]) + "<br></td>"
+			temp = temp + "</tr>"
+		temp = temp + "</table>" + body_tail + "</body></html>"
+		return temp
+
+
+
+
+
+
+	def change_number_to_tel_style(self, input_value):
+		# 전화번호나 핸드폰 번호 스타일을 바꿔주는것
+		# 전화번호를 21345678 =>02-134-5678 로 변경하는 것
+		result = input_value
+		value = str(int(input_value))
+		if len(value) == 8 and value[0] == "2":
+			# 22345678 => 02-234-5678
+			result = "0" + value[0:1] + "-" + value[1:4] + "-" + value[4:]
+		elif len(value) == 9:
+			if value[0:2] == "2":
+				# 223456789 => 02-2345-6789
+				result = "0" + value[0:1] + "-" + value[1:5] + "-" + value[5:]
+			elif value[0:2] == "11":
+				# 113456789 => 011-345-6789
+				result = "0" + value[0:2] + "-" + value[2:5] + "-" + value[5:]
+			else:
+				# 523456789 => 052-345-6789
+				result = "0" + value[0:2] + "-" + value[2:5] + "-" + value[5:]
+		elif len(value) == 10:
+			# 5234567890 => 052-3456-7890
+			# 1034567890 => 010-3456-7890
+			result = "0" + value[0:2] + "-" + value[2:6] + "-" + value[6:]
+		return result
+
+
+
+	def split_sentence(self, input_list1d, base_words):
+		# 문장으로 된것을 의미있는 단어들로 분리하는 것
+		aaa = collections.Counter()
+		for one in input_list1d:
+			value = str(one).lower().strip()
+			if len(value) == 1 or value == None or value == " ":
+				pass
+			else:
+				for l1 in base_words:
+					value = value.replace(l1[0], l1[1])
+				value = value.replace(",", " ")
+				value = value.replace("(", " ")
+				value = value.replace(")", " ")
+				value = value.replace("  ", " ")
+				value = value.replace("  ", " ")
+				values = value.split(" ")
+				aaa.update(values)
+		return aaa
+
+	def del_set_item_by_list(self, input_set, input_list):
+		"""
+		list의 항목으로 들어간것을 하나씩 꺼내어서
+		set안에 같은것이 있으면 지운다
+		"""
+		for one in input_list:
+			input_set.remove(one)
+		return input_set
+
+
+	def change_set_item_by_list(self, input_set, input_list2d):
+		"""
+		input_list = [["변경전자료1", "변경후자료2"], ["변경전자료11", "변경후자료22"], ]
+		"""
+		for list_1d in input_list2d:
+			input_set.discard(list_1d[0])
+			input_set.add(list_1d[1])
+		return input_set
+
+	def zzz_sample_1(self):
+		# 자주 사용하는 함수의 갯수를 알아내는 것이다
+		num = 0
+		result = []
+		for one in ["pcell.py", "youtil.py", "jfinder.py", "anydb.py", "ganada.py", "mailmail.py", "pynal.py",
+		            "pyclick.py", "scolor.py"]:
+			aaa = self.change_python_file_to_sorted_by_def(one)
+			num = num + len(aaa)
+			result.append([one, len(aaa)])
+		print(num)
+		print(result)
+
+	def count_function_num_in_python_file(self, python_file_list):
+		#원하는 python화일안에 몇개의 def로 정의된 메소드가 있는지 확인하는 것이다
+		result = []
+		num = 0
+		for one in python_file_list:
+			aaa = self.change_python_file_to_sorted_by_def(one)
+			num = num + len(aaa)
+			result.append([one, len(aaa)])
+		result.append(["총갯수는 ===>", num])
+		return result
+
+	def print_one_by_one(self, input_list):
+		for one in input_list:
+			print(one)
+
+	def filter_not_empty_value_in_list2d_by_index_no(self, input_list2d, index_no=4):
+		# index 번호의 Y열의 값이 빈것이 아닌것만 돌려주는 것
+		result = []
+		for index, one in enumerate(input_list2d):
+			if one[index_no]:
+				result.append(one)
+		return result
+
+	def get_cho_sung_for_korean(self, input_kor):
+		# 초성의 글자만 갖고오는것
+		result = []
+		for one in input_kor:
+			try:
+				aa = self.split_jamo_in_korean(one)
+				result.append(aa[0][0])
+			except:
+				pass
+		return result
+
+	def change_file_to_list_by_def(self, filename):
+		result = {}
+		def_text = ""
+		def_name = ""
+		f = open(filename, "r", encoding="UTF8")
+		lines = f.readlines()
+		for one_text in lines:
+			if str(one_text).strip()[0:3] == "def":
+				if not def_name == "":
+					result[def_name] = def_text
+				def_name = str(one_text).strip()[3:].split("(")[0]
+				def_text = def_text + one_text
+		return result
+
+	def get_unique_function_between_two_python_file(self, file_a, file_b):
+		a_file = self.change_file_to_list_by_def(file_a)
+		b_file = self.change_file_to_list_by_def(file_b)
+		a_file_keys = a_file.keys()
+		b_file_keys = b_file.keys()
+		unique_a = []
+		for one_key in a_file_keys:
+			if not one_key in b_file_keys:
+				unique_a.append([a_file_keys])
+		return unique_a
+
+	def add_serial_value(self, input_list2d, start_no=1, special_char =""):
+		#2 차원값의 값의 제일 처음값에만 순서가있는 값을 넣기
+		#값의 맨앞에 1), 2), 3)과같은 순서의 값을 넣고 싶을때
+		for x in range(len(input_list2d)):
+			if not start_no =="":
+				add_value = str(start_no+x) + special_char
+			else:
+				add_value = special_char
+			input_list2d[x][0] = add_value + input_list2d[x][0]
+		return input_list2d
+
+	def easy_format(self, input_value, big_digit="", small_digit="", comma="", fill_char="", left_right=""):
+		small_digit_value = small_digit
+		if left_right == "left":
+			left_right_value = ""
+		elif left_right == "right":
+			left_right_value = ">"
+		else:
+			left_right_value = ""
+
+		if small_digit != "":
+			small_digit_value = "." + str(small_digit) + "f"
+		format_string = left_right_value + fill_char + str(big_digit) + comma + small_digit_value
+		result = format(input_value, format_string)
+		return result
+
+
+	def sort_list2d_by_index(self, input_list2d, index_no=0):
+		"""
+		입력 :  리스트자료
+		리스트자료를 몇번째 순서를 기준으로 정렬하는것
+		숫자와 문자가 같이 섞여 있어도, 정렬이 가능
+		aa = [[111, 'abc'], [222, 222],['333', 333], ['777', 'sjpark'], ['aaa', 123],['zzz', 'sang'], ['jjj', 987], ['ppp', 'park']]
+		value=sort_list(리스트자료, 정렬기준번호)
+		"""
+
+		none_temp = []
+		str_temp = []
+		int_temp = []
+		for list1d in input_list2d:
+			if type(list1d[index_no]) == type(None):
+				none_temp.append(list1d)
+			elif type(list1d[index_no]) == type("str"):
+				str_temp.append(list1d)
+			else:
+				int_temp.append(list1d)
+
+		result_int = sorted(int_temp, key=lambda x: x[index_no])
+		result_str = sorted(str_temp, key=lambda x: x[index_no])
+		result = none_temp + result_int + result_str
+		return result
+
+	def sort_list3d_by_index(self, input_list3d, index_no=0):
+		result = []
+		for input_list2d in input_list3d:
+			if len(input_list2d) == 1:
+				result.append(input_list2d)
+			else:
+				sorted_list2d = self.sort_list2d_by_index(input_list2d, index_no)
+				result.append(sorted_list2d)
+		return result
+
+	def group_input_list2d_by_index_no(self, input_list2d, index_no=4):
+		result = []
+		sorted_input_list2d = self.sort_list2d_by_index(input_list2d, index_no)
+		check_value = sorted_input_list2d[0][index_no]
+		temp = []
+		for one_list in sorted_input_list2d:
+			if one_list[index_no] == check_value:
+				temp.append(one_list)
+			else:
+				result.append(temp)
+				temp = [one_list]
+				check_value = one_list[index_no]
+		if temp:
+			result.append(temp)
+		return result
+
+	def group_input_list3d_by_index_no(self, input_list3d, index_no=4):
+		result = []
+		for input_list2d in input_list3d:
+			sorted_input_list2d = self.sort_list2d_by_index(input_list2d, index_no)
+			grouped_list3d = self.group_input_list2d_by_index_no(sorted_input_list2d, index_no)
+			result = result + grouped_list3d
 		return result
```

### Comparing `xython-1.3.0/src/xython.egg-info/PKG-INFO` & `xython-1.4.0/src/xython.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,140 @@
 Metadata-Version: 2.1
 Name: xython
-Version: 1.3.0
+Version: 1.4.0
 Summary: Easy Read / Write for Excel, Word, Color, Etc using Python
 Home-page: https://github.com/sjpark/xython
-Download-URL: https://github.com/sjpark/xython/archive/v1.3.0.tar.gz
 Author: sjpark
 Author-email: sjpkorea@yahoo.com
+License: UNKNOWN
+Download-URL: https://github.com/sjpark/xython/archive/v1.4.0.tar.gz
+Description: ## xython 모듈에 대하여
+        ### 개괄적인 설명
+        이모듈은 업무용으로 많이 사용하는 엑셀 , 색, 정규표현식, 등에 대하여 Python과 win32com을 기본으로 사용하여 각기 새롭게 모듈을 만들어서 좀더 쉽고 편하게 사용하고 만들자는 것입니다
+        자동화는 각자의 사용에 대한  
+        
+        만든 이유는 우리가 업무등을 하는 입장에서, 손으로 작업하기에는 양이 많고, 그렇다고
+        계속 반복적으로 일어나는 일은 아니며, VBA등을 만들어서 사용하기에는 어렵고 힘든 부분에 대해서
+        
+        파이썬이라는 훌룡한 언어를 위용하여, 좀더 쉽고 간결하게 몇가지 기능만 배워도 20줄안으로 자신만의 코드를
+        만들어 사용할수있는 기준을 만들기 위한 것입니다
+        
+        또한 보통 많이 사용하는 코드들은 첨부된 sample코드를 보시거나 저의 사이트에 와서 비슷한것을 다운 받은후
+        변경해서 사용하시기를 추천 드립니다
+        
+        좀더 편한 업무의 일을 하기위한 것입니다
+        
+        ### 구성은 
+        
+            - pcell : 엑셀을 다루는 것
+            - pcell_event : 엑셀의 이벤트를 다루는것
+            - scolor : 색의 RGB값을 편하게 사용가능하도록 만든 것
+            - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
+            - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
+            - ganada : 워드를 다루기위해 만든 것
+            - mailmail : outlook을 다루는것
+            - pyclick : 키보드와 마우스를 다루는 모듈
+            - pynal : 시간과 날짜를 다루는것
+            - youtil : 이러저런 문장이나 시간등을 변환하는데 도움이되는 것
+            - basic_data : halmoney패키지에서 사용되는 전반적인 공유 자료들을 저장하는 곳
+        
+        각 사용사용방법들에 대해서는 아래의 사이트를 참고하세요
+        
+        * https://cafe.naver.com/pycell
+        * www.halmoney.com
+        * www.xython.co.kr
+        
+        
+        ## 기본 사용법
+        ### pcell
+        -각 메소드는 각각 별도의 내용으로 사용합니다
+        
+        Pcell의 모듈을 만들 때 나름대로 편하고 쉽게 이름을 만들려고 하였습니다. 기본적인 틀을 만들어 놓으니, 분명억지로 지어진 이름또한 있음을 시인합니다. 나름대로 생각하고 고심한끝에 만들어진 이름이오니 맘에 들지 않는 부분이 있이더라도 양해를 부탁드립니다
+        
+        물론, 지금의 이름이 최종이라고는 생각하지 않고 있습니다. 좋은 이름이라는것은 어떤 메소드가 들어가 있는지 잘 몰라도 거의 사용하는데 사람의 생각에서 쉽게 사용을 할수 있도록 만드는 것이라고 생각을 합니다
+        
+        아마 한 4~5번정오는 크게 이름을 변경한 것 같습니다. 만들어놓고 조금지나면 저스스로가 도데체 이것의 이름은 왜 이렇게 만들어놓은거야???라는 질문을 하는경우가 가끔있습니다. 이리바꾸고 저리바꾸어도 맘에 안드는구석이 아직 많습니다
+        
+        한사람의 이름이 인생에서 차지하는부분이 많듯이 제가만든것또한 그러하지만, 만약 맘에 안드시는 것이 있으시면 본인스스로가 바꾼어서 사용하셔도 됩니다
+        
+        단, 기존의것은 그대로 두시고 아래부분에 새로운 메소드를 추가하셔서 위의것을 그대로 사용하시면 될것입니다
+        
+        그래서 다음과 같은 원리를 이용해서 만들었으나, 조금은 틀린부분도 있지만…
+        
+        	1. 이름은 기본적으로 3부분으로 만들었으며 각부분은 언더바(_)로 연결했습니다
+        	2. 읽을때는 read, 쓸때는 write, 삭제는 delete, 추가는insert등을 사용하였습니다
+        	3. 두번째의 이름의 규칙은
+        		관련된 부분에 따라 다른것을 사용하며 다음과 같은 것이 사용이 됩니다
+        		거진 영역을 나타내는 부분으로 사용하였습니다
+        		range, workbook, cell, line, column
+        	4. 세번째 부분이 어떤 일을 할것인지를 알아보는 것입니다
+        	5. 일반사항은 다음과 같습니다
+        
+        -	모든함수에는 sheet가 명시되어야 합니다
+        -	값을 읽는것은 read로 시작하며
+        -	값을 쓰는 것은 write로 시작합니다
+        -	선을 긋는등의 그림은 dwg로 시작합니다
+        -	하나의 자료가 아닌, 자료의 묶음은 Range를 사용한다
+        -	두개의 문구사이에는 '_' 로 연결을 하였다 예) read_cell
+        -	메소드는 모두 소문자를 사용함
+        
+        예를 들어, 어떤셀에 값을 입력하는 것은 write_value_in_cell라는 이름으로 구성하였습니다
+        그리고 부가적으로 함수의 변수로 사용되는부분은 큰 것->작은것으로 만들었으며, 영역을 표시하는 부분은 모두 리스트를 기준으로 하나로 만들었습니다.
+        
+        그저, 그렇다는것을 이해바라며, 실질적으로 코드를 보시면 더 쉽게 이해가 가실것으로 생각됩니다.
+        보지않고 찾지않아도 함수의 이름을 생각해낼수있도록 만든다고 나름대로 정의한 것입니다.
+        
+        ### scolor
+        이것은 모든 외부로 들어오고 나가는 것은 전부 RGB형태로 이루어지도록 만든다
+        
+            - 색을 변경하고 관리하는 모듈이며
+            - 색의 변화를 잘 사용이 가능하도록 하기위한 것이다
+            - 기본 입력 예 : "빨강", "빨강55", "red55", "0155"
+            - 기본색 ==> 12색 + (하양, 검정, 회색),
+            - 큰변화 ==> 1~9단계, 작은변화 ==> 1~9단계
+            - 기본함수 : get_color_rgb("red55"), get_rgb_3input(색, 큰변화, 작은변화)
+            - 모든 색의 표현이나 결과는 rgb로 돌려준다
+        
+        ### Jfinder
+        이름을 **Jfinder**라고 지었으며, 아래와 같은 특성을 가지고 있다
+        
+        1. 건수는 ~를 사용하여 4~5라는 식으로 표현을 하였고
+        2. 한글, 영어와 같은 것은 대괄호를 사용하여 적용하였다 [한글]
+        3. 처음과 끝은 [처음], [끝]처럼 나타냈다
+        4. 그리고 이것은 누가 보아도 아~~ 무엇을 찾을려고 했는지를 알수있도록 하기위한것이며
+        5. 찾기기능중에 전부 찾아서 보기쉽도록 돌려주는 것과 같은 몇가지 메소드들을 만들어 넣었읍니다
+        제일 중요한 코드를 만드는 기능은 아래와 같읍니다
+        대략적으로 위의것을 읽은후에 보시면 이해가 되실부분이 많읍니다
+        
+        * 아래의 코드들은 정규표현식을 사용하면서, 내가 만든 표현식조차도 다시 읽기가 어려워서, 나름 다른 형태로 만들어 본것인데. 생각보다 가독성이 좋아서 같이 공유해보는것이다
+        또한 만든김에 결과로 돌려주는것도 하나만 받으면 전부 가능하도록 만들어 보았다
+        위에서 언급한 이메일 형식이 맞느지를 보는 것은 상당히 반복적이기 때문에 크게 혼돈은 없다
+        하지만, 실제 코드를 사용하다 보면, 외계어를 해석하는 상태까지 와야할 경우가 있다
+        
+        
+            ([a-zA-Z0-9_.+-]+)@[a-zA-Z0-9_.+-]+\.[a-zA-Z0-9_.+-]+
+        
+        * 이정도만해도 간단한 축에 속한다. 맨처음 만들때는 그나마 이해를 하지만, 다른사람이 만든 것을 이해하는데 상당한 시간이 걸린다는 것이고, 또한 일반적인 사용자들이 이것을 공부하고 이해하는데 어려움이 잇을 것 같으면서 동시에, 정규표현식의 강력함을 사용할수 있도록 생각해 보는 것이다
+        그래서 좀더 간단하게 사용법을 만들고,
+        
+        
+            [영어&숫자.+-:1~]@[영어&숫자.+-:1~]\.[영어&숫자.+-:1~]
+        이렇게 바꾸면 좀더 읽기가 쉬워진다
+        
+        **jfinder**에는 자주사용하는 언어를 등록할수도 있읍니다. 예를 들어 일본어나 한자를 등록한것처럼 하면 사용이 가능하다.
+        간단하게 다시 사용하는 방법을 알려주면, 너무 줄여놓은 정규표현식을 좀더 늘이는 것이라고 생각하면 됩니다. 여기에서 느낀 부분은 전문가가 사용하기에는 좋지만, 비전문가가 사용하기 쉽게, 예전에는 단어1개가 아주 중요한 속도까지 영향을 주지만, 지금은너무 줄이지 않아도 된다는 것이다. 기계에 가까운 언어에서 좀더 사용자에 가까운 언어로 만들어도 된다는 것이지요
+        파이선이 사용하기에 좀더 편한방법이 되는 것이지요
+        
+            - 대괄호로 묶는다
+            - 반복갯수는 대괄호안에 사용하며 ~로 나타낸다
+            - 맨처음 맨마지막등의 용어는 [처음], [끝]등의 이유로 나타낸다 
+            - 특수문자(re모듈내에 의미가있는 문자)는 \를 붙여서 사용한다
+            - 어떤문자의 앞과뒤에있을때는 (앞에있음:abc)이라고 사용하면 abc가 앞에있는 문자열을 찾는것이다
+        
+        ### mailmail
+        이름을 **mailmail**라고 지었으며, 아웃룩의 이메일을 관리하는 도구입니다
+        - 이것의 장점은 엑셀이나 Util과 연동하여 편의성을 더욱 증대하고있읍니다
+        - 기본적인 사용법이나 함수의 이름은 같은 형태를 따릅니다
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-
-## xython 모듈에 대하여
-### 개괄적인 설명
-이모듈은 업무용으로 많이 사용하는 엑셀 , 색, 정규표현식, 등에 대하여 Python과 win32com을 기본으로 사용하여 각기 새롭게 모듈을 만들어서 좀더 쉽고 편하게 사용하고 만들자는 것입니다
-자동화는 각자의 사용에 대한  
-
-만든 이유는 우리가 업무등을 하는 입장에서, 손으로 작업하기에는 양이 많고, 그렇다고
-계속 반복적으로 일어나는 일은 아니며, VBA등을 만들어서 사용하기에는 어렵고 힘든 부분에 대해서
-
-파이썬이라는 훌룡한 언어를 위용하여, 좀더 쉽고 간결하게 몇가지 기능만 배워도 20줄안으로 자신만의 코드를
-만들어 사용할수있는 기준을 만들기 위한 것입니다
-
-또한 보통 많이 사용하는 코드들은 첨부된 sample코드를 보시거나 저의 사이트에 와서 비슷한것을 다운 받은후
-변경해서 사용하시기를 추천 드립니다
-
-좀더 편한 업무의 일을 하기위한 것입니다
-
-### 구성은 
-
-    - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
-    - basic_data : halmoney패키지에서 사용되는 전반적인 공유 자료들을 저장하는 곳
-    - ganada : 워드를 다루기위해 만든 것
-    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
-    - mailmail : outlook을 다루는것
-    - pcell : 엑셀을 다루는 것
-    - pcell_event : 엑셀의 이벤트를 다루는것
-    - pyclick : 키보드와 마우스를 다루는 모듈
-    - pynal : 시간과 날짜를 다루는것
-    - scolor : 색의 RGB값을 편하게 사용가능하도록 만든 것
-    - youtil : 이러저런 문장이나 시간등을 변환하는데 도움이되는 것
-
-각 사용사용방법들에 대해서는 아래의 사이트를 참고하세요
-
-* https://cafe.naver.com/pycell
-* www.halmoney.com
-
-
-## 기본 사용법
-### pcell
--각 메소드는 각각 별도의 내용으로 사용합니다
-
-Pcell의 모듈을 만들 때 나름대로 편하고 쉽게 이름을 만들려고 하였습니다. 기본적인 틀을 만들어 놓으니, 분명억지로 지어진 이름또한 있음을 시인합니다. 나름대로 생각하고 고심한끝에 만들어진 이름이오니 맘에 들지 않는 부분이 있이더라도 양해를 부탁드립니다
-
-물론, 지금의 이름이 최종이라고는 생각하지 않고 있습니다. 좋은 이름이라는것은 어떤 메소드가 들어가 있는지 잘 몰라도 거의 사용하는데 사람의 생각에서 쉽게 사용을 할수 있도록 만드는 것이라고 생각을 합니다
-
-아마 한 4~5번정오는 크게 이름을 변경한 것 같습니다. 만들어놓고 조금지나면 저스스로가 도데체 이것의 이름은 왜 이렇게 만들어놓은거야???라는 질문을 하는경우가 가끔있습니다. 이리바꾸고 저리바꾸어도 맘에 안드는구석이 아직 많습니다
-
-한사람의 이름이 인생에서 차지하는부분이 많듯이 제가만든것또한 그러하지만, 만약 맘에 안드시는 것이 있으시면 본인스스로가 바꾼어서 사용하셔도 됩니다
-
-단, 기존의것은 그대로 두시고 아래부분에 새로운 메소드를 추가하셔서 위의것을 그대로 사용하시면 될것입니다
-
-그래서 다음과 같은 원리를 이용해서 만들었으나, 조금은 틀린부분도 있지만…
-
-	1. 이름은 기본적으로 3부분으로 만들었으며 각부분은 언더바(_)로 연결했습니다
-	2. 읽을때는 read, 쓸때는 write, 삭제는 delete, 추가는insert등을 사용하였습니다
-	3. 두번째의 이름의 규칙은
-		관련된 부분에 따라 다른것을 사용하며 다음과 같은 것이 사용이 됩니다
-		거진 영역을 나타내는 부분으로 사용하였습니다
-		range, workbook, cell, line, column
-	4. 세번째 부분이 어떤 일을 할것인지를 알아보는 것입니다
-	5. 일반사항은 다음과 같습니다
-
--	모든함수에는 sheet가 명시되어야 합니다
--	값을 읽는것은 read로 시작하며
--	값을 쓰는 것은 write로 시작합니다
--	선을 긋는등의 그림은 dwg로 시작합니다
--	하나의 자료가 아닌, 자료의 묶음은 Range를 사용한다
--	두개의 문구사이에는 '_' 로 연결을 하였다 예) read_cell
--	메소드는 모두 소문자를 사용함
-
-예를 들어, 어떤셀에 값을 입력하는 것은 write_value_in_cell라는 이름으로 구성하였습니다
-그리고 부가적으로 함수의 변수로 사용되는부분은 큰 것->작은것으로 만들었으며, 영역을 표시하는 부분은 모두 리스트를 기준으로 하나로 만들었습니다.
-
-그저, 그렇다는것을 이해바라며, 실질적으로 코드를 보시면 더 쉽게 이해가 가실것으로 생각됩니다.
-보지않고 찾지않아도 함수의 이름을 생각해낼수있도록 만든다고 나름대로 정의한 것입니다.
-
-### scolor
-이것은 모든 외부로 들어오고 나가는 것은 전부 RGB형태로 이루어지도록 만든다
-
-    - 색을 변경하고 관리하는 모듈이며
-    - 색의 변화를 잘 사용이 가능하도록 하기위한 것이다
-    - 기본 입력 예 : "빨강", "빨강55", "red55", "0155"
-    - 기본색 ==> 12색 + (하양, 검정, 회색),
-    - 큰변화 ==> 1~9단계, 작은변화 ==> 1~9단계
-    - 기본함수 : get_color_rgb("red55"), get_rgb_3input(색, 큰변화, 작은변화)
-    - 모든 색의 표현이나 결과는 rgb로 돌려준다
-
-### Jfinder
-이름을 **Jfinder**라고 지었으며, 아래와 같은 특성을 가지고 있다
-
-1. 건수는 ~를 사용하여 4~5라는 식으로 표현을 하였고
-2. 한글, 영어와 같은 것은 대괄호를 사용하여 적용하였다 [한글]
-3. 처음과 끝은 [처음], [끝]처럼 나타냈다
-4. 그리고 이것은 누가 보아도 아~~ 무엇을 찾을려고 했는지를 알수있도록 하기위한것이며
-5. 찾기기능중에 전부 찾아서 보기쉽도록 돌려주는 것과 같은 몇가지 메소드들을 만들어 넣었읍니다
-제일 중요한 코드를 만드는 기능은 아래와 같읍니다
-대략적으로 위의것을 읽은후에 보시면 이해가 되실부분이 많읍니다
-
-* 아래의 코드들은 정규표현식을 사용하면서, 내가 만든 표현식조차도 다시 읽기가 어려워서, 나름 다른 형태로 만들어 본것인데. 생각보다 가독성이 좋아서 같이 공유해보는것이다
-또한 만든김에 결과로 돌려주는것도 하나만 받으면 전부 가능하도록 만들어 보았다
-위에서 언급한 이메일 형식이 맞느지를 보는 것은 상당히 반복적이기 때문에 크게 혼돈은 없다
-하지만, 실제 코드를 사용하다 보면, 외계어를 해석하는 상태까지 와야할 경우가 있다
-
-
-    ([a-zA-Z0-9_.+-]+)@[a-zA-Z0-9_.+-]+\.[a-zA-Z0-9_.+-]+
-
-* 이정도만해도 간단한 축에 속한다. 맨처음 만들때는 그나마 이해를 하지만, 다른사람이 만든 것을 이해하는데 상당한 시간이 걸린다는 것이고, 또한 일반적인 사용자들이 이것을 공부하고 이해하는데 어려움이 잇을 것 같으면서 동시에, 정규표현식의 강력함을 사용할수 있도록 생각해 보는 것이다
-그래서 좀더 간단하게 사용법을 만들고,
-
-
-    [영어&숫자.+-:1~]@[영어&숫자.+-:1~]\.[영어&숫자.+-:1~]
-이렇게 바꾸면 좀더 읽기가 쉬워진다
-
-**jfinder**에는 자주사용하는 언어를 등록할수도 있읍니다. 예를 들어 일본어나 한자를 등록한것처럼 하면 사용이 가능하다.
-간단하게 다시 사용하는 방법을 알려주면, 너무 줄여놓은 정규표현식을 좀더 늘이는 것이라고 생각하면 됩니다. 여기에서 느낀 부분은 전문가가 사용하기에는 좋지만, 비전문가가 사용하기 쉽게, 예전에는 단어1개가 아주 중요한 속도까지 영향을 주지만, 지금은너무 줄이지 않아도 된다는 것이다. 기계에 가까운 언어에서 좀더 사용자에 가까운 언어로 만들어도 된다는 것이지요
-파이선이 사용하기에 좀더 편한방법이 되는 것이지요
-
-    - 대괄호로 묶는다
-    - 반복갯수는 대괄호안에 사용하며 ~로 나타낸다
-    - 맨처음 맨마지막등의 용어는 [처음], [끝]등의 이유로 나타낸다 
-    - 특수문자(re모듈내에 의미가있는 문자)는 \를 붙여서 사용한다
-    - 어떤문자의 앞과뒤에있을때는 (앞에있음:abc)이라고 사용하면 abc가 앞에있는 문자열을 찾는것이다
```

