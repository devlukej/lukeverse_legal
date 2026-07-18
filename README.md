# lukeverse_legal

편한하루(lukeverse_bus) 앱의 스토어 등록정보(Google Play Console 등)에 연결하는
개인정보처리방침 / 이용약관 공개 페이지입니다.

- 이 저장소는 **공개(Public)**로 유지해야 GitHub Pages 무료 호스팅이 동작합니다.
- 내용은 `D:\Project\lukeverse_bus\server\app\legal_pages.py` 를 기준으로 생성됩니다.
  문구를 바꿀 때는 그 파일을 수정한 뒤, 아래 명령으로 다시 생성하세요.

```bash
python -c "
import sys
sys.path.insert(0, r'D:\Project\lukeverse_bus\server')
from app.legal_pages import render_privacy_policy_html, render_terms_html
open('index.html', 'w', encoding='utf-8').write(render_privacy_policy_html())
open('terms.html', 'w', encoding='utf-8').write(render_terms_html())
"
```

## 배포된 URL (GitHub Pages + 커스텀 도메인)
- 개인정보처리방침: https://bus-legal.lukeverse.com/
- 이용약관: https://bus-legal.lukeverse.com/terms.html

(커스텀 도메인 연결 전에는 https://devlukej.github.io/lukeverse_legal/ 로도 접근 가능)
