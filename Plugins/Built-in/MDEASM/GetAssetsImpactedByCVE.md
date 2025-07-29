📅 2025.07.29

<img width="349" height="310" alt="image" src="https://github.com/user-attachments/assets/c384c3a5-88d6-40ae-a5fb-9b1b329ceaac" />

# 🛠️ 여러 개의 CVE를 입력할 때 유의할 JSON 형식 처리 방법

보안 분석 도구나 API를 사용할 때, 사용자로부터 **CVE(Common Vulnerabilities and Exposures)** 목록을 입력받는 경우가 많습니다.  
이때, 여러 개의 CVE 값을 한 번에 입력하려면 **JSON 형식을 준수해야 하며**, 특히 형식 오류로 인해 데이터가 제대로 처리되지 않는 문제가 자주 발생합니다.

---

## 🔍 문제 상황

빈칸에 다음과 같이 CVE를 입력했다고 가정해보겠습니다:

CVE-2023-12345, CVE-2024-23456, CVE-2025-34567


겉보기에 보기 좋지만, **JSON 포맷에서는 유효하지 않은 형식**입니다. 이 형태는 일반 텍스트이며, JSON 파서가 인식할 수 없습니다.

---

## ✅ 올바른 JSON 형식

JSON 배열로 CVE 여러 개를 입력하려면 다음과 같은 형식을 따라야 합니다:

```json
"CVE-2023-12345", "CVE-2024-23456", "CVE-2025-34567"
```
