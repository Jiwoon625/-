# 전세 보증금 예측 Streamlit 앱

## 준비
1) 모델 파일 `jeonse_gbm_xgb.json`을 이 폴더에 복사.
2) 가상환경 생성 후 의존성 설치:

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate

pip install -r requirements.txt
```

## 실행
```bash
streamlit run app.py
```

브라우저가 열리면 주소 입력 후 "지도/좌표 업데이트" 버튼을 누르고, 필요 시 지도에서 클릭으로 위치를 조정한 뒤 **예측하기**를 눌러 결과를 확인하세요.

## 참고
- 지오코딩은 Nominatim을 사용하므로 과도한 호출을 피하세요.
- 카테고리 인코딩은 `app.py` 상단 `ENCODING`에서 조정 가능합니다.
