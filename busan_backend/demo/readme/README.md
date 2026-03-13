네, 수정된 모든 사항(Spring Boot 3.x, Thymeleaf, PostgreSQL, Docker Hub 배포 등)을 반영하여 GitHub에 바로 복합해서 사용할 수 있도록 정리해 드립니다.

아래 박스 안의 내용을 전체 복사하여 `README.md` 파일에 붙여넣으세요.

---

```markdown
# 🌊 부산 문화관광 웹 애플리케이션 (Busan Culture & Tourism)

부산의 아름다운 관광 명소와 다채로운 문화 정보를 제공하는 **Spring Boot 3.x** 기반의 웹 서비스 프로젝트입니다.

## 🔗 프로젝트 링크 (Project Links)
* **Live Demo (GitHub Pages):** [바로가기](https://jihwana120.github.io/)
* **Project Documentation (Notion):** [상세 산출물 보기](https://coconut-truck-1db.notion.site/77bcdef944a1837599cc01e60077313a?source=copy_link)
* **Docker Hub Repository:** [like1324/busan:1.0](https://hub.docker.com/r/like1324/busan)

---

## 👥 팀원 소개 (Team 2)
| 성명 | 역할 | 담당 업무 |
| :--- | :--- | :--- |
| **안민수** | **Team Leader** | 프로젝트 총괄, Spring Boot 백엔드 및 서비스 로직 개발 |
| **박주환** | **DevOps & Developer** | **Docker Image 빌드 및 Cloud 배포(Docker Hub)**, DB 아키텍처 설계 |
| **김승민** | Team Member | HTML/CSS 기반 프런트엔드 UI 디자인 및 Thymeleaf 연동 |
| **최정민** | Team Member | 데이터 정제 및 PostgreSQL 쿼리 작성, 백엔드 기능 구현 |

---

## 🛠 기술 스택 (Tech Stack)

### **Backend**
* **Framework:** Java 17 / Spring Boot 3.x
* **View Engine:** Thymeleaf (Server-side Template Engine)
* **Database:** PostgreSQL

### **Frontend**
* **UI/UX:** HTML5, CSS3 (Vanilla UI)

### **Infrastructure & Deployment**
* **Deployment:** Docker / Docker Hub (Containerization)
* **Version Control:** Git / GitHub (Source Code Hosting)

---

## 🚀 주요 기능 (Key Features)
1. **부산 관광 정보 제공:** Spring Boot와 PostgreSQL을 연동한 동적 관광 명소 데이터 조회
2. **서버 사이드 렌더링:** Thymeleaf를 활용하여 효율적이고 안정적인 데이터 바인딩 구현
3. **심플하고 직관적인 UI:** 별도의 프레임워크 없이 HTML/CSS만으로 최적화된 화면 구성
4. **컨테이너 기반 배포:** Docker Hub를 통해 배포된 이미지를 활용하여 클라우드 및 서버 환경에 즉각 배포 가능

---

## ⚙️ 실행 방법 (Run Instructions)

### **1. Source Code로 실행**
```bash
# 레포지토리 클론
git clone [https://github.com/jihwana120/jihwana120.github.io.git](https://github.com/jihwana120/jihwana120.github.io.git)
cd jihwana120.github.io

# application.properties에서 PostgreSQL 연결 정보 확인 후 실행
./gradlew bootRun

```

### **2. Docker를 이용한 실행**

배포 담당자(박주환)가 Docker Hub에 업로드한 이미지를 사용하여 즉시 구동할 수 있습니다.

```bash
# Docker Hub에서 이미지 다운로드
docker pull like1324/busan:1.0

# 컨테이너 실행 (8080 포트 기준)
docker run -d -p 8080:8080 --name busan-app like1324/busan:1.0

```

---

## 📂 프로젝트 구조 (Directory Structure)

* `src/main/java/`: Spring Boot 백엔드 컨트롤러, 서비스, 엔티티
* `src/main/resources/templates/`: Thymeleaf 기반 HTML 템플릿 파일
* `src/main/resources/static/`: CSS 디자인 파일 및 이미지 리소스
* `Dockerfile`: 컨테이너 빌드를 위한 설정 파일

---

### 📄 라이선스 (License)

본 프로젝트는 교육 및 포트폴리오 목적으로 제작되었습니다.

```

---

**Tip:** 혹시 `application.properties` 파일에 DB 비밀번호나 민감한 정보가 포함되어 있다면, 배포 시에는 환경변수로 처리하거나 `.gitignore`에 등록하는 것이 좋습니다. 추가로 문서화할 내용이 있으면 언제든 말씀해 주세요!

```