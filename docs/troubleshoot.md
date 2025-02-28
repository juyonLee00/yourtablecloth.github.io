# 식탁보 문제 해결

## 샌드박스가 닫히면서 "현재 연결은 원격 호스트에 의해 강제로 끊겼습니다" 오류 메시지가 나타납니다.

Windows Sandbox는 사용자와 상호 작용하는 부분을 Remote Desktop Protocol (RDP)을 이용하여 구현했습니다. 그러나 일부 보안 소프트웨어들은 RDP를 통한 서비스 사용을 의도적으로 차단합니다.

![Windows Sandbox가 강제 종료된 상황](images/SandboxError.png)

이 문서에서는 가장 잘 알려진 사례인 AhnLab Safe Transaction (이하 AST) 프로그램의 사례에 대한 해결 방법을 안내합니다. 다른 소프트웨어의 경우, 해당 소프트웨어 제조사에 문제 해결을 요청해야 할 수 있습니다.

![AhnLab Safe Transaction에서 나타내는 메시지](images/ASTError.png)

AST가 RDP를 강제 종료하지 않게 설정을 변경하려면 다음과 같이 설정을 바꿉니다.

1. 작업 표시줄의 트레이 아이콘 영역에서 방패 모양의 AST 아이콘을 마우스 오른쪽 버튼으로 클릭합니다.
1. 팝업 메뉴에서 **Settings** 메뉴를 클릭합니다.
1. 설정 대화 상자가 나타나면, **System Security** 탭을 클릭합니다.
1. **Block remote access** 체크 상자를 해제합니다.
1. **Close** 버튼을 클릭합니다.
1. 보안이 취약해질 수 있다는 경고 메시지가 나타나면, **Yes** 버튼을 눌러 설정 변경에 동의합니다.

## 해당 오류가 발생하는 기관
아래 기관들 중 일부를 사용할 경우, 식탁보를 실행하기 전 미리 설정을 바꿔 놓는 것을 권장합니다.
- KDB 산업은행
- 카카오뱅크
- BNK부산은행
- 한국투자증권
- MG새마을금고
- 애큐온저축은행
- 메리츠증권
- 한국투자증권
- 하나금융투자
- 케이프투자증권
- KB국민카드
- 삼성생명

---

[되돌아가기](index.md)
