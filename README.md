# vote-dashboard

간편하게 `votes.html`을 공유·확인할 수 있는 대시보드입니다.

- 미리보기 링크(iframe 우회): https://htmlpreview.github.io/?https://raw.githubusercontent.com/sesacs/vote-dashboard/main/votes.html
- 원본 raw 파일: https://raw.githubusercontent.com/sesacs/vote-dashboard/main/votes.html

사용법
- 위 미리보기 링크를 그대로 공유하면 브라우저에서 바로 렌더링됩니다.
- 파일을 수정한 뒤에는 `git push`까지 완료해야 링크에 최신 내용이 반영됩니다.
- 리더보드 크롤링이 CORS로 막힐 경우, `cors.isomorphic-git.org`, `api.allorigins.win`, `r.jina.ai` 등의 프록시를 순차 재시도하며, 그래도 실패하면 캐시된 스냅샷(`data/leaderboard.html`)을 사용합니다.
- `.github/workflows/update-leaderboard.yml`가 매시간 스냅샷을 갱신하려고 시도합니다. 모두 차단될 경우에는 로컬(example.py)에서 실행하거나 수동으로 `data/leaderboard.html`을 업데이트해야 합니다.
