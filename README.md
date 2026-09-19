<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Key Learning & Reflection</title>
</head>
<body>
<h2>Service Topic</h2>
<p>데이터 관리를 할 수 있는 CRUD 프론트엔드 웹페이지이다.</p>
<h2>주제 설명</h2>
    <p>이번 과제는 반응형 웹사이트를 만드는 것에 초점을 두어 external css도 사용하여 전반적인 상품목록관리(추가,삭제,수정, 조회)를 할 수 있는 웹 페이지를 만들었습니다. </p>
   <h2>List Page</h2>
    <p>Required 필수 입력해야 하는 항목을 만들었습니다. 이름,제목 들들 주요 필드가 비어있지 않도록 했습니다.</p>
    <p>Email Format 올바른 이메일 형식인지 확인해서 입력받을 수 있도록 하였습니다.</p>
    <p>Min Length 입력값의 최소 글자 수를 2글자로 설정해서 2글자 이상만 입력받을 수 있도록 했습니다.</p>
    <p>Min Length 입력값의 최소 글자 수를 2글자로 설정해서 2글자 이상만 입력받을 수 있도록 했습니다.</p>
    <p>Select Validation 카테고리나 상태값 선택 시 기본옵션이 아닌 유효한 값을 선택했는지 확인할 수 있도록 했습니다.<p>

<h2>RWD</h2>
    <p>Bootstrap의 Grid System과 Flexbox를 최대한 활용하여 데스크탑과 모바일 환경 모두에서 최적화된 UI/UX를 제공합니다.</p>
    <P>Desktop 환경: 왼쪽 280px 고정 폭의 Sidebar와 오른쪽 Main Content 영역이 병렬(d-flex)로 배치했습니다. 카드(Album) 및 테이블 목록이 3열(row-cols-md-3) 이상으로 여유 있게 출력됩니다.</P>
    <p>Mobile 환경: 화면 폭이 줄어들면 Navigation 메뉴 및 Sidebar 요소가 수직으로 배치되거나 축소됩니다. 카드 목록이 1열(row-cols-1)로 자동 전환되어 작은 화면에서도 스크롤하며 편하게 볼 수 있습니다.</p>
    
<h2>AI Usage: AI를 어떤 부분에 활용했으며, 생성된 코드를 어떻게 확인/수정했는지 작성</h2>
    <p>디테일하게 수정해야 부분들 글씨체가 뭔지, 몇 픽셀 수정해야 정확하게 일치하는지 줄 바꾸는 법 등등 활용했고 결정적으로 도움을 받은 부분은 과제 마칠 때쯤 사이드바에도 마우스를 올리면 링크타서 이동할 수 있고 색도 바뀐다는 걸 알게 돼서 마우스 올렸을 때 디자인 주는 방법hover를 AI를 통해 배웠습니다. 그리고 sementic 태그 없이도 특정 한 줄을 타겟할 수 있다는 것도 알게 되었습니다.</p>

 <h2>Bootstrap Components & Classes</h2>
    <p>components들로는 Navbar, Header로 상단에 홈페이지 바로가기, 상품등록, 상품 목록 으로 갈 수 있는 메뉴로 구성했고,
    Footer로 하단 주요 링크 및 카피라이트 표기했고, Buttons & Button Groups으로 주요 동작(View, Edit, Delete 등)을 할 수 있는 버튼을 만들었습니다.</p>
    <p>사용한 class로는 d-flex, flex-grow-1, flex-shrink-0로 가변할 수 있는 레이아웃을 만들었고, row-cols-1, row-cols-sm-2, row-cols-md-3들로 반응형 그리드 시스템을 만들었습니다.</p>

 <h2>Problem & Solutions</h2>
    <p>index.html 구현 중 메인 콘텐츠(카드 목록) 하단에 와야 할 Footer가 카드 목록 위에 출력되고, 사이드바와 레이아웃이 어긋나는 현상이 발생했습니다.</p>
    <p>사이드바와 메인 콘텐츠 영역을 감싸는 div.d-flex 태그가 카드 목록 영역 전체를 포함하기 전에 일찍 닫혔고, footer가 카드 목록보다 먼저 배치되어서 발생한 구조문였습니다.</p>
    <p>footer를 전체 페이지 최하단으로 이동시키고, 카드 목록(album) 영역을 메인 콘텐츠 영역(flex-grow-1) 안으로 위치시켜 원래의 의도대로 나올 수 있도록 하였습니다.</p>
</body>
</html>
