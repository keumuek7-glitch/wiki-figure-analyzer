# 위인 분석 카드

위키백과(한국어·영어·일본어)나 나무위키의 인물 문서 본문을 붙여넣으면 다음을 분석하는 정적 웹페이지입니다.

1. 인물 이력서
2. MBTI 추정 (축마다 'I 6 대 4 E'처럼 비율 표시)
3. 성격 장단점
4. 성공·실패 요인
5. 인생 육각형: 업적, 영향력, 리더십, 도덕성, 인간관계, 역경 극복 (가중치 1:1:1:1:1:1)

실존 인물과 가상 인물(소설·애니메이션·만화·게임) 모드, 원문 인용 확인, 일본어 등 외국어 본문 분석과 번역을 지원합니다.

## 본인 API 키로 사용 (BYOK)

이 사이트에는 서버가 없습니다. 이용자가 화면에 넣은 **Google Gemini** 또는 **Anthropic Claude** API 키로, 이용자의 브라우저가 AI 회사 API를 직접 호출합니다.

- 키는 사이트 운영자에게 전송되거나 저장되지 않습니다.
- 기본적으로 탭을 닫으면 지워지고(sessionStorage), '이 기기에 키 기억하기'를 켠 경우에만 브라우저 localStorage에 남습니다.
- 사용 요금은 키 주인에게 청구됩니다.
- `netlify.toml`의 Content-Security-Policy가 외부 연결을 `api.anthropic.com`과 `generativelanguage.googleapis.com`으로만 제한합니다.

키 발급: [Google AI Studio](https://aistudio.google.com/apikey) / [Anthropic Console](https://console.anthropic.com/settings/keys)

## 배포

빌드 과정이 없는 단일 `index.html`입니다. Netlify에 이 저장소를 연결하면 그대로 배포됩니다(publish 디렉터리 `.`).
