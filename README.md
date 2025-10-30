# SAP_UI5-Fiori-
SAP UI5를 공부하는 곳(공식 튜토리얼)


-----
## [Stap 4] XML View
모든 UI 코드를 index.js에 넣으면 나중에 관리가 힘들어진다. 따라서 XML View를 쓰면 UI 구조를 선언적으로 쓸 수 있고 JS와 분리되어 관리가 쉬워진다.
-> 선언적으로 쓴다는 말은 무엇인가?
" 결과적으로 어떻게 보여질지를 코드에서 설명만 해서 자동으로 만들게 하는 방식이라는 말이다.
에를 들어 아래와 같이 명령형의 코드를 봐보면
`let text = new Text();
text.settext("안녕하세요");
text.placeAt("content");`
이러면 내가 직접 객체를 만들고 속성을 세팅하고 위치를 지정해야한다.

하지만 선언형으로 했다면? 어떤 구조로 보여달라고 선언만 하면 실제 동작은 프레임워크가 알아서 만들어 준다.
`<mvc:View xmlns="sap.m" xmlns:mvc="sap.ui.core.mvc">
  <Text text="안녕하세요"/>
<mvc:View>`
Text라는 것이 있고 텍스트는 안녕하세요 라고 구성만 선언한다.
실제로 어디에 어떻게 뭘로 만들지는 SAPUI5가 알아서 처리하면 된다.
