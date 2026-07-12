# web — 정적 화면

이 폴더만 Cloudflare Pages / Vercel / Netlify 에 올리면 바로 사이트가 됩니다.
빌드 과정이 없습니다. Build command는 비워두세요.

  index.html      상품 목록 (첫 화면)
  p.html          상품 상세
  m.html          모바일
  checklist.html  출산 준비물 체크리스트
  admin.html      관리자 — ⚠️ Cloudflare Access 로 반드시 잠글 것

지금은 화면 안에 가짜 데이터가 들어 있습니다.
server 를 띄운 뒤, 각 파일의 <script> 안 상수(ITEMS, SELLERS 등)를
fetch('https://api.내도메인/products') 로 바꾸면 실제 데이터가 흐릅니다.
