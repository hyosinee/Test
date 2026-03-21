# 🎓 Git & GitHub 실습 프로젝트

> Git과 GitHub의 기본 흐름을 직접 손으로 익히기 위한 실습 저장소입니다.

---

## 📌 목표

- Git 기본 명령어 익히기 (`init`, `add`, `commit`, `log` 등)
- GitHub 원격 저장소 연결 및 `push` / `pull` 실습
- 브랜치 생성 및 병합 (`branch`, `merge`) 실습
- 충돌(conflict) 발생 및 해결 경험

---

## 📁 파일 구성

| 파일명 | 설명 |
|---|---|
| `README.md` | 프로젝트 소개 (이 파일) |
| `hello.py` | 간단한 Python 실습 파일 |
| `calculator.py` | 기능 추가 실습용 계산기 파일 |
| `notes.txt` | 자유롭게 수정해보는 메모 파일 |
| `.gitignore` | Git이 추적하지 않을 파일 목록 |

---

## 🚀 실습 순서 (추천)

### 1단계 — 로컬 저장소 초기화
```bash
git init
git add .
git commit -m "첫 번째 커밋: 초기 파일 추가"
```

### 2단계 — GitHub 원격 저장소 연결
```bash
git remote add origin https://github.com/사용자명/저장소명.git
git push -u origin main
```

### 3단계 — 파일 수정 후 커밋
```bash
# notes.txt 파일을 수정한 뒤
git add notes.txt
git commit -m "notes.txt 내용 업데이트"
git push
```

### 4단계 — 브랜치 실습
```bash
git branch feature/add-greeting   # 브랜치 생성
git checkout feature/add-greeting  # 브랜치 이동
# hello.py 수정 후
git add .
git commit -m "인사말 기능 추가"
git checkout main
git merge feature/add-greeting     # 병합
```

### 5단계 — 원격에서 변경사항 가져오기
```bash
git pull origin main
```

---

## 📝 자주 쓰는 명령어 요약

```bash
git status          # 현재 상태 확인
git log --oneline   # 커밋 이력 간단히 보기
git diff            # 변경사항 확인
git stash           # 작업 임시 저장
```

---

*Happy Coding! 🐙*
