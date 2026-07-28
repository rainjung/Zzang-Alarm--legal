# Zzang Alarm — Legal

강제 기상 알람 앱 **Zzang Alarm**의 이용약관·개인정보처리방침을 GitHub Pages로 게시하는 저장소.

공개 URL: <https://rainjung.github.io/Zzang-Alarm--legal/>

## 구조

```
index.md                 언어 선택 랜딩
ko/terms.md  ko/privacy.md
en/terms.md  en/privacy.md
ja/terms.md  ja/privacy.md
_layouts/default.html    공용 레이아웃(자체 CSS · 외부 테마 의존 없음)
_config.yml              kramdown(GFM) 설정
```

## 원본과 동기화

한국어판의 **원본은 앱 저장소**에 있다 — `Alarm-JJang/docs/이용약관.md`,
`docs/개인정보처리방침.md`. 내용을 고칠 때는 원본을 먼저 고치고 이곳에 반영한다
(front matter만 덧붙이면 된다). 영어·일본어판은 이 저장소가 원본이다.

## 게시 설정

GitHub → Settings → Pages → Source: **Deploy from a branch** → `main` / `/ (root)`

## 갱신 시 확인

- 시행일(`최종 업데이트`)을 함께 올린다 — 3개 언어 6개 파일 모두.
- 앱 내 설정 화면의 링크가 위 URL을 가리키는지 확인한다.
- 운영자·사업자등록번호·문의처가 바뀌면 6개 파일 + `index.md` + 레이아웃 푸터를 모두 고친다.
