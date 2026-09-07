# MUMUN CLASS

고등학교 미술 수업자료. 정적 HTML, 빌드 없음.

## 구조
```
index.html          목록
mimesis/index.html  01 미메시스
<slug>/index.html   새 주제는 폴더 하나 추가 후 index.html 목록에 한 줄
```

## 배포 (Cloudflare Pages)
1. GitHub에 `mumun_class` 리포 만들고 이 폴더 push
2. Cloudflare 대시보드 → Workers & Pages → Create → Pages → Connect to Git → 리포 선택
3. Build settings: Framework `None`, Build command 비움, Output directory `/`
4. Deploy 후 Custom domains → `class.mumun.xyz` 추가 (DNS CNAME 자동 생성)

이후엔 `git push` 만 하면 1분 내 반영.

## 도판 원칙
- 퍼블릭 도메인 / CC0 / CC BY-SA 만 내장 (base64)
- 저작권 보호 작품(폴록 등)은 싣지 않고 미술관 페이지 링크
- 출처는 각 페이지 footer에 표기
