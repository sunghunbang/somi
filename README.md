# 면접분석기 (interview-analyzer)

미술 세특·활동을 입력하면 서류 진단, 예상 질문(시행착오·성찰 심화), 스스로 공부할 것을 자동으로 정리해 주는 웹앱입니다. 서버 없이 브라우저에서만 동작하며, `index.html` 파일 하나로 완결됩니다.

## 배포 방법 (GitHub Pages)

1. GitHub에서 새 저장소 생성 → 이름을 **interview-analyzer** 로 지정 (Public)
2. 이 폴더의 `index.html` 파일을 저장소 루트에 업로드 (Add file → Upload files)
3. 저장소 **Settings → Pages** 이동
4. Source를 **Deploy from a branch**, Branch를 **main / (root)** 로 선택 후 Save
5. 1~2분 뒤 아래 주소에서 접속 가능
   - `https://[GitHub계정명].github.io/interview-analyzer/`
   - 예: `https://sunghunbang.github.io/interview-analyzer/`

## 사용법 요약

- **① 입력**: 활동명·유형·키워드와 7단계(동기~확장) 내용을 작성
- **② 진단·핵심질문**: 빈칸/모호한 표현을 자동 진단하고, 시행착오·성찰 심화 질문·꼬리질문 사슬 확인
- **③ 스스로 공부**: 우선순위별 학습 과제 체크리스트, 60~90초 답변 프레임, Claude 검토용 프롬프트 복사
- 왼쪽 사이드바에서 여러 활동을 추가·관리 가능
- **전체 인쇄 · PDF 저장**: 모든 활동을 한 번에 인쇄/PDF로 출력 (일괄)
- **개별 파일로 저장 (ZIP)**: 활동별 Markdown 파일 + 전체 요약을 ZIP으로 일괄 저장
- **전체 JSON 저장 / 불러오기**: 작업 내용을 JSON으로 백업하거나 이어서 작업

모든 데이터는 브라우저 안에서만 처리되며 외부로 전송되지 않습니다.

## 학생별 버전 (예: somi.html)

`somi.html`은 권소미 학생의 미활보(교과 세특 6건 · 비교과 6건)를 미리 입력해 둔 버전입니다. 같은 저장소에 `index.html`과 함께 올려두면 됩니다.

- 위 1~4단계로 만든 저장소(interview-analyzer)에 `somi.html`을 그대로 추가 업로드
- 접속 주소: `https://[GitHub계정명].github.io/interview-analyzer/somi.html`
- 다른 학생도 같은 방식으로 만들려면: 앱에서 빈 `index.html`을 열어 학생별로 입력 → 왼쪽 "전체 JSON 저장"으로 백업하거나, `somi.json` 같은 형식의 파일을 만들어 요청하면 미리 채워진 `[학생명].html`을 만들어 드릴 수 있습니다.
- `somi.json`은 위 12개 활동의 원본 데이터입니다. 다른 사본에서 "JSON 불러오기" 버튼으로 그대로 불러와 이어서 입력할 수 있습니다.

⚠️ 미활보 원문에 시행착오·해결·전공 연결 서술이 부족한 항목은 해당 칸을 비워 두었습니다(내용을 지어내지 않았습니다). 앱의 ② 진단 탭에서 "빈칸"으로 표시되는 부분이 바로 인터뷰 전 보완이 필요한 지점입니다.
