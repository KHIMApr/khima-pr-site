# KHIMA 홍보위 발행물 사이트

KHIMA 홍보위원회 발행물(정책 카드뉴스·이슈페이퍼·뉴스레터)의 공개 아카이브입니다.

- 홈(`index.html`) = 호수별 아카이브 인덱스 — 데이터는 `archive-data.js`에서 관리
- 발행물 페이지는 `/2026/<호수>/` 경로에 추가 (URL 영구 고정)
- 게시 = 사람이 push/merge (검증·게시는 사람 원칙)
- 공개 페이지의 모든 사실 항목은 검증된 원기관 원문으로 연결: 사실 블록에 `data-source-required`, 클릭 가능한 링크에 `class="source-link"`, `target="_blank"`, `rel="noopener noreferrer"` 사용
- 원문 URL이 없거나 링크 확인에 실패한 항목은 게시하지 않음
- 디자인 토큰(`tokens.css`)은 작업 레포 `디자인시스템/tokens.css`와 동기 유지


## main 보호와 자동 링크 생성

`main`은 관리자에게도 PR을 강제하고 force-push·브랜치 삭제를 금지한다. 승인 리뷰 수는 0이므로 `Association_PR/도구_우분투자동화/publish.sh`가 provenance·내용·asset 검사를 통과한 감사 PR을 즉시 merge할 수 있다. 스크립트 밖에서 main에 직접 push하지 않는다. 게시 후 검증 실패는 해당 merge만 별도 rollback PR로 되돌린다.
