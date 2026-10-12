# 월간 다이어리 (monthly-diary)

종이 월간 다이어리(Plan · CSF · Road Map · Routine · Schedule)를 아이폰에서 쓰는 앱.
김익한 교수 영상 2개(월간 다이어리 사용법, 60일 다이어리 챌린지)의 쓰는 법을 각 탭 "쓰는 법"에 정리했다.

- 주소: https://yeonheekim-prog.github.io/monthly-diary/
- 저장: localStorage 키 `monthlyDiary_v1` (월별 `months["YYYY-MM"]`)
- 페이지 9장(위쪽 목차): 자기선언 / 달력 / 인생지도 / 월간계획 / 로드맵 / 루틴 / 주간 / 데일리 / 메모 — 종이 다이어리 사진과 같은 배치
- 데이터: `months["YYYY-MM"]`, `weeks["월요일 날짜"]`(tasks[8], cells{"줄-요일":{t,s}}), `days["YYYY-MM-DD"]`, `decl`. 메뉴(⋯)에서 백업
- 폰·PC 동기화: 비공개 저장소 yeonheekim-prog/monthly-diary-data 의 diary.json 하나를 함께 씀(GitHub API, 기기마다 fine-grained 토큰 1회 입력, localStorage `monthlyDiary_sync`). 칸(달·주·날·자기선언)마다 고친 시각 `D.mt`가 최신인 쪽을 남김. 연결 직전 기록은 `monthlyDiary_presync`에 보관
