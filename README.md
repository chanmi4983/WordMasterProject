Word Master Project 나찬미 1분반 전산심화학부 222002402023.09.16

프로젝트 github repo 
 https://github.com/chanmi4983/WordMasterProject

프로그램 설명 및 제작 목적
단어장을 관리하는 프로그램입니다. ICRUD 인터페이스를 구현하며 단어 및 단어 목록 생성, 읽기, 업데이트, 삭제인 CRUD의 기본 기능들을 가지고 있으며 파일을 저장하고 읽어올 수 있고 데이터로 저장 가능 하도록 하여 보다 더 효율적으로 단어를 관리할 수 있습니다.

개발 환경: 깃허브, 이클립스

구현 기능과 목록:
1.	addWord()
   <img width="143" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/997bf21d-102c-4916-b43c-d397d37a3fc1">

 
목적: 단어(word)와 뜻(meaning)을 입력 받고 단어를 추가합니다.
구현: 난이도, 단어, 뜻을 입력 받아 Word 객체를 생성한 후. 객체를 list에 추가하여 새로운 단어를 사전에 저장한다.
2.	listAll() 
<img width="136" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/180b887d-561e-460a-8fa0-af1ade1c35da">

 
목적: 단어를 모두 입력한 순서대로 혹은 파일에 있는 모습 그대로 목록을 화면에 보여준다..
구현: list에 있는 모든 Word 객체를 출력하여 각 단어에 대한 정보는 단어의 난이도, 단어 자체, 뜻으로 구성

3.	listAll(int level) 메서드:
 <img width="219" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/1c246553-acc5-4c9a-a0c9-47a1f39abf2d">

목적: 특정 난이도의 단어만 나열하여 출력합니다.
구현:list에 있는 모든 Word 객체를 반복하면서 난이도가 지정된 level과 일치하는 단어만 출력합니다. 각 단어에 대한 정보는 단어의 난이도, 단어 자체, 뜻으로 구성되어 화면에 표시

4.	listAll(String keyword):
목적: 특정 키워드를 포함하는 단어만 나열하여 사용자에게 표시합니다.
구현: list에 있는 모든 Word 객체를 반복하면서 단어가 지정된 keyword를 포함하는 경우만 출력, 각 단어에 대한 정보는 단어의 난이도, 단어 자체, 뜻으로 구성되어 화면에 표시됩니다.일치하는 단어의 인덱스 목록을 반환합니다.
5.	updateItem():
  <img width="174" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/520b20d7-29b5-40c8-84b7-c4fe440ff065">
<img width="187" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/8633ccf3-9e26-4e58-bdd5-89022f73cf03">


목적: 사용자가 선택한 단어의 뜻을 수정합니다.
구현: 수정할 단어를 검색하여 일치하는 모든 단어를 출력한 후, 수정할 단어의 인덱스를 선택하고, 새로운 뜻을 입력하여 수정하고나서 단어의 뜻을 업데이트하여 변경 내용을 저장합니다.
6.	deleteItem() 
  <img width="151" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/a4266f7b-5f8a-4822-ac78-228445a86546">
<img width="155" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/e8ef4b05-d22f-4583-88a2-9d74b5b5578e">


목적: 사용자가 선택한 단어를 삭제합니다.
구현: 삭제할 단어를 검색색하고 일치하는 모든 단어를 보여준다. 사용자가 삭제할 단어의 인덱스를 선택하고, 삭제 여부를 확인합니다. 사용자가 확인한 경우, 선택한 단어를 list에서 제거하여 삭제합니다.
<img width="209" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/79b2a9c5-7f02-437e-a4b6-5998fb3afbe7">

  7, 8번 동시에 활용됨
7.	loadFile():
목적: 사전 데이터를 파일에서 읽어와서 list에 띄운다.
구현: 파일에서 데이터를 읽어와서 각 라인을 추출 하여 Word 객체로 변환시킨 후 list에 추가합니다.
8.	saveFile():
목적: 단어 목록을 파일에 저장
구현:list에 있는 모든 Word 객체를 파일에 저장하기 위해 문자열 형식으로 변환하여 파일에 쓰고 저장합니다.
9.	searchLevel()
: <img width="202" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/ee91c3a0-5376-4ff3-bcbf-808edbb7d468">

목적: 사용자가 원하는 난이도의 단어만 표시합니다.
구현: 사용자로부터 원하는 난이도를 입력 받고 해당되는 난이도와 단어만 출력합니다.
10.	searchWord():
 <img width="174" alt="image" src="https://github.com/chanmi4983/WordMasterProject/assets/102154392/13f4e868-c358-4430-b3f5-3959e1d97a69">

•	목적: 사용자가 원하는 특정 단어를 검색하여 표시합니다.
구현: 사용자로부터 원하는 단어 혹은 그 단어의 들어간 철자를 입력 받고 해당 단어를 포함하는 단어만 출력합니다.
![image](https://github.com/chanmi4983/WordMasterProject/assets/102154392/3b2df669-adb5-4a1c-9df5-aad8dc4a451a)
