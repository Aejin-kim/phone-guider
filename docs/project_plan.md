# 프로젝트 계획: 카카오 T 택시 연습하기 앱

## 프로젝트 개요
카카오 T 택시 연습하기 앱의 웹 인터페이스를 구현하는 프로젝트입니다.

## 주요 목표
1. 실제 카카오 T 앱과 유사한 사용자 경험 제공
2. 모바일 친화적인 반응형 디자인 구현
3. 터치 인터랙션 최적화
4. 택시 호출 프로세스 시뮬레이션

## 프로젝트 구조
```
phone/
├── index.html                    # 메인 페이지
├── destination-input.html        # 도착지 입력 페이지 (드래그 가능한 택시 아이콘 포함)
├── destination-search.html       # 도착지 검색 페이지 (제주공항 검색 시 특별 처리)
├── jeju-airport-results.html    # 제주공항 검색 결과 페이지
├── taxi-call.html               # 택시 호출 페이지
├── taxi-call-complete.html      # 택시 호출 완료 페이지
├── docs/                        # 프로젝트 문서
│   ├── project_phone.md         # 프로젝트 진행 상황
│   └── project_plan.md          # 프로젝트 계획서
└── images/                      # 이미지 파일들
```

## 완료된 작업

### 1. 메인 페이지 (index.html) ✅
- 카카오 T 로고 및 메인 타이틀 구현
- 4개 연습 버튼 구현 (택시 호출, 택시 취소, 카드 등록, 한번에 연습)
- 반응형 디자인 및 애니메이션 효과 적용

### 2. 도착지 입력 페이지 (destination-input.html) ✅
- 지도 컨테이너 구현
- 드래그 가능한 택시 아이콘 추가
- "출발" 라벨이 포함된 택시 아이콘
- 마우스 및 터치 드래그 지원
- 지도 경계 내에서만 이동 가능

### 3. 도착지 검색 페이지 (destination-search.html) ✅
- 검색 입력 필드 및 음성 검색 버튼
- 빠른 접근 버튼 (집, 회사, 현재위치)
- "제주공항" 검색 시 jeju-airport-results.html로 자동 이동
- 일반 검색은 destination-input.html로 이동

### 4. 제주공항 검색 결과 페이지 (jeju-airport-results.html) ✅
- 제주공항 주변 5개 주요 시설 정보 표시
- 각 시설별 아이콘, 이름, 주소, 거리 정보
- 택시 호출 및 길찾기 버튼
- 순차적 애니메이션 효과
- 모바일 최적화된 반응형 디자인

## 기술적 특징

### 드래그 앤 드롭 기능
- 마우스 및 터치 이벤트 지원
- 지도 경계 내 제한된 이동
- 부드러운 드래그 경험

### 검색 및 라우팅
- 키워드 기반 페이지 이동
- URL 파라미터를 통한 데이터 전달
- 뒤로가기 기능 지원

### UI/UX 디자인
- 카카오 T 앱과 유사한 디자인 언어
- 일관된 색상 체계 및 타이포그래피
- 터치 친화적 버튼 크기 및 간격
- 부드러운 전환 애니메이션

## 다음 단계
1. 택시 호출 페이지 (taxi-call.html) 기능 구현
2. 택시 호출 완료 페이지 (taxi-call-complete.html) 구현
3. 전체 플로우 테스트 및 사용성 개선
4. 성능 최적화 및 접근성 향상

## 기술 스택
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **디자인**: Flexbox, CSS Grid, CSS Animations
- **반응형**: Mobile-first approach, Media queries
- **인터랙션**: Touch events, Drag & Drop, Event handling

## 브라우저 지원
- Chrome (최신 버전)
- Safari (최신 버전)
- Firefox (최신 버전)
- Edge (최신 버전)
- 모바일 브라우저 (iOS Safari, Chrome Mobile)

## 프로젝트 상태
- **진행률**: 70%
- **현재 단계**: 핵심 페이지 구현 완료
- **다음 마일스톤**: 택시 호출 플로우 완성
