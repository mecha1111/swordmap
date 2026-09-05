# 프리마 맵 에디터

퍼즐 액션 플랫포머 **(가제) 성검을 얻었는데 몸이 약하다**의 웹 레벨 에디터.
브라우저에서 맵을 만들고 물리로 테스트한 뒤 JSON·캡처로 프로그래머에게 전달합니다.

## 파일 구조
```
index.html       진입점 (마크업)
style.min.css    스타일
app.min.js       에디터 로직
assets.js        타일셋·스프라이트 (base64)
matter.min.js    물리 엔진 (Matter.js)
```

## 로컬 실행
정적 파일이라 서버 없이 index.html을 브라우저로 열면 됩니다.
(일부 브라우저는 file:// 제한이 있으니 `python3 -m http.server`로 열면 확실합니다.)

## 배포 (GitHub Pages)
1. 이 폴더 전체를 리포지토리에 올림
2. Settings → Pages → Source: main / root
3. `https://<아이디>.github.io/<리포>/` 접속

## 조작
- **B** 붓 · **U** 사각채우기 · **D** 지우개 · **V** 선택·이동 · **F** 전체보기
- **Space** 재생/정지 · **Ctrl+Z / Ctrl+Y** 되돌리기
- 재생 중: **← →** 이동 · **Z** 점프 · **X** 공격

> 재생 물리는 참고용이며 실제 유니티와 다를 수 있습니다.
