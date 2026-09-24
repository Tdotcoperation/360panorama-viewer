# 360 Panorama Viewer

Cloudflare Workers 기반 파노라마/360° 이미지 뷰어입니다.

- 로컬 이미지 선택/드래그 앤 드롭
- `?url=https://example.com/panorama.jpg` 로 원격 이미지 자동 로드
- 원격 이미지는 `/proxy?url=...` Workers 프록시를 통해 CORS와 무관하게 로드
- 좌우 무한 회전, 확대/축소, 자동 회전, 연결부 블렌딩
- 모바일 더블 탭 / PC 더블클릭 또는 F 키로 전체화면

## 배포

```bash
npm install
npx wrangler login
npm run deploy
```

> 브라우저가 디코딩할 수 없는 특수 이미지 코덱은 표시되지 않을 수 있습니다. 프록시는 보안을 위해 로컬/사설 네트워크 주소를 차단합니다.
