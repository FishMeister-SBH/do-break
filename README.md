# 두부레이크 · Do Break

흰 큐브를 당겼다 놓아 건물을 와장창 부수는 미니멀 3D 게임이에요. 브라우저에서 바로 돌아가고, 폰에서는 터치로 드래그하면 돼요.

- **퍼즐**: 직접 설계한 8개 레벨을 가장 적은 드래그로 전부 부수기
- **자유 모드**: 서울 강남역 · 여의도, 뉴욕 미드타운의 실제 건물을 90초 동안 부수기
- 메인 메뉴에서는 고르고 싶은 모드의 건물을 부수면 돼요.

## 실행

정적 파일만 있으면 돼요. `index.html`과 `city.json`을 같은 폴더에 두고 아무 웹 서버로 열면 됩니다.

```bash
python -m http.server 8000
```

## 사용한 것

- [three.js](https://threejs.org) 0.160 (MIT), jsDelivr CDN에서 불러와요.
- 지도 데이터 © [OpenStreetMap](https://www.openstreetmap.org/copyright) 기여자, [ODbL](https://opendatacommons.org/licenses/odbl/) 라이선스. `city.json`은 이 데이터를 가공한 파생 데이터베이스로, 같은 ODbL을 따라요.
- 글꼴 [Pretendard](https://github.com/orioncactus/pretendard) (SIL Open Font License 1.1). 페이지에 쓰인 글자만 뽑아 `index.html`에 넣었어요.
