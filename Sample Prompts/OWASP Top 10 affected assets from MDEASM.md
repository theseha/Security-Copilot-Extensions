📅 2025.07.29

<img width="562" height="782" alt="image" src="https://github.com/user-attachments/assets/b26c7b7e-be66-439c-8156-39c340e8e7d0" />

# 🔍 Security Copilot에서 MDEASM 데이터를 활용한 답변 예시와 Markdown 응답 형식

Microsoft Security Copilot은 자연어로 입력된 보안 관련 질문에 대해 풍부한 데이터 기반의 분석과 정형화된 결과를 제공할 수 있습니다. 특히, 특정 소스(Microsoft Defender 제품군 등)를 명시적으로 지시함으로써 **보다 정확한 인사이트**를 얻을 수 있습니다.

---

## 🎯 명확한 데이터 소스 지시: "MDEASM" 참조

아래와 같은 프롬프트를 Security Copilot에 입력한 경우를 생각해보겠습니다:


이 요청은 다음 두 가지 중요한 요소를 포함하고 있습니다:

1. **데이터 출처 명시**: `MDEASM (Microsoft Defender External Attack Surface Management)` 를 명확히 언급함
2. **응답 형식 지정**: Markdown 테이블로 결과를 보여달라는 형식 요청

Copilot의 실행 로그 중 `Chose Microsoft Defender External Attack Surface Management` 메시지를 통해, 해당 데이터 소스가 올바르게 참조된 것을 확인할 수 있습니다.

---

## 🧾 단순 텍스트에서 벗어나 Markdown 테이블 사용하기

보통 보안 분석 보고서를 만들거나 팀과 협업할 때는 단순한 문장 나열보다는 **구조화된 데이터 형식**이 필요합니다.  
이때 `Markdown`은 Copilot에게 다음과 같은 포맷을 지정해줄 수 있는 유용한 도구입니다:

- 표(Table)
- 강조 및 구분선 등

---

## ✅ 예시: Copilot이 반환한 Markdown 테이블

아래는 실제로 Copilot이 생성한 Markdown 테이블 형식의 응답 예시입니다:

```markdown
| **OWASP Top 10 List ** | **Asset Name** | **Asset Type** |
|----------------------------------------------------------------| 
| A01: Broken Access Control | ZavaDB | DB |
| A02: Cryptographic Failure | JWR Secret Key | Key |
```
