해냈다...!!!


대박사건.
오늘 하루종일 도르마무처럼 다시 시작하느라 죽을맛이였는데 구현된 결과물을 보니 날아갈 것 같다.
![image](https://github.com/user-attachments/assets/1176d603-75c6-4304-884e-30ec1eb680a9)

아무 노드나 열어서 주피터노트북과 클라우드쉘을 활용해 
아래단계부터 빌드업하는 과정을 진행했다.
기본적인 pip install부터 막혔었는데, uvicorn과 fastapi를 설치해주고,

$cd aiffel/fastAPI
$python server_fastapi_vgg16.py

를 통해 하위폴더와 서버를 열어준다. 서버를 연다! 의 개념 이제는 알 것 같아!ㅠㅠ

이후에 클라우드 쉘 2개를 열어, 둘중 하나만 ngrok 토큰을 적용시키고(이때 반드시 중괄호는 뗄 것)

$python server_fastapi_1.py
$ngrok http 5000
을 각각 실행시킨다.

후자의 URL을 기본 크롬 주소창에 치면, 웹화면이 구현되는데 이때.docs를 붙이면, 예상한 결과화면이 나온다.

이 화면의 주소를 FlutLab에 구현된 애뮬레이터에 입력해도 이집트캣 몇프로 결과가 나오게 된다.

웹릴리즈 해서 깃헙에 올리는 과정은 조원들의 도움을 많이 받았는데,
일단 기존의 레포지토리가 아닌 새로운 레포지토리를 만들어주는 것 부터 시작한다.
vgg16_api_tutorial이라는 새 레포지토리를 만든다.
setting/pages 항목에서 branch를 'main'으로 변경해주고,
index.html 파일에서 
base를 <base href="/vgg16_api_tutorial/">로 편집해준다. (이때 /를 앞뒤로 닫아주는 것이 포인트!)

셋팅의 주소를 클릭하면 실행완료!
아까의 URL 입력해도 같은 값 이집트고양이,0.3086..뜬다! 올레!!

진짜 너무너무 스트레스받고 어려운 작업이였는데,
어떻게 이렇게 기본도 다시 모르고 헤매나 싶었는데 
막상 다 하고 나니까 되게 뿌듯했다.
도움주신 퍼실님과 조원들께 정말 감사드리고 
앞으로도 잘 안되는것도 끝까지 지지부진하게라도 물고 늘어져봐야겠다고 생각했다. 아이펠 화이팅!
