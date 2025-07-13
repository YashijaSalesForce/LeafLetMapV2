# 야쉬자맵V2(Event,Opportunity APEX 구현완료 & 현재위치 구현완료)
<img width="1232" alt="image" src="https://github.com/user-attachments/assets/22669428-9f7a-44b7-8f53-021dd121483c" />

# 모바일 버전
## 기능1. Event,Account,Opportunity,Campaign 표시
<img width="338" height="73" alt="image" src="https://github.com/user-attachments/assets/ef39fdb3-0ca1-4130-8f68-7f306b12f560" />

## 기능2. 본사 및 현재위치
<img width="335" height="398" alt="image" src="https://github.com/user-attachments/assets/0adc376a-5eb8-45bb-8906-b5844d8c86e2" />
<img width="329" height="399" alt="image" src="https://github.com/user-attachments/assets/4a22daab-8a0e-4b04-9c51-38260bafcb67" />

## 기능3. 일정(Event) 목록 불러오기 / 위치 안내
#### 해당 영업사원(User)의 Event 목록을 전부 표시
<img width="347" height="242" alt="image" src="https://github.com/user-attachments/assets/ef295a6e-5fbe-4731-8c2f-ebe6ef1e1021" />

#### 위치 안내 선택 시
<img width="332" height="512" alt="image" src="https://github.com/user-attachments/assets/c3af6ff6-fd11-43da-8475-80e2a33698b6" />

## 기능4. 전화/경로안내
#### 전화번호가 null이 아니면 전화버튼 활성화
<img width="341" height="506" alt="image" src="https://github.com/user-attachments/assets/3bc43bf9-f01b-4cfe-93f0-4c8147e2d9c4" />

#### 경로안내 버튼 클릭시 카카오맵으로 경로안내
<img width="345" height="583" alt="image" src="https://github.com/user-attachments/assets/f9e2a014-1445-4c72-bfff-828114b07916" />
<img width="342" height="587" alt="image" src="https://github.com/user-attachments/assets/1d3dacc1-d842-4ac7-af2b-8d0d57738bcd" />


# 필요한 세팅
### 1. 다운로드
Leaflet CSS 다운로드
https://unpkg.com/leaflet@1.9.4/dist/leaflet.css 접속
Leaflet JS 다운로드
https://unpkg.com/leaflet@1.9.4/dist/leaflet.js 접속

### 2. Static Resources 업로드
Setup → Static Resources → New
1) css파일
Name: leafletCSS
File: 방금 저장한 leaflet.css 파일 선택
Cache Control: Public
2) js 파일
Name: leafletJS
File: 방금 저장한 leaflet.js 파일 선택
Cache Control: Public

### 3. Trusted URLs 등록(CSP 설정)
![image](https://github.com/user-attachments/assets/6e2593ef-7301-460e-90a5-bb5c17534f84)
`SetUp->Trusted URL and Browser Policy Violations`에서 violation에 걸린거 확인 후 추가.


### 주의사항
- 파일명은 정확히 leaflet.css, leaflet.js로 저장
- Static Resource Name은 leafletCSS, leafletJS로 입력
- 파일 확장자 빠뜨리지 않기
- CSP 설정(Trusted URLs) 빠뜨리지 않기

