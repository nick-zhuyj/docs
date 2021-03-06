---

copyright:
  years: 2015,2016

---

{:new_window: target="\_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}
{:pre: .pre}

# 보안 정책 구성
{: #set_up_policies.md}
마지막 업데이트 날짜: 2016년 11월 15일
{: .last-updated}

보안 분석가는 연결 보안 정책과 블랙리스트 또는 화이트리스트를 구성할 수 있습니다. 

## 연결 정책 구성

모든 디바이스에 적용되는 기본 보안 레벨을 설정할 수 있습니다. 그런 다음 특정 디바이스에 대한 사용자 정의 보안 설정을 추가할 수 있습니다. 

1. 위험 및 보안 관리 추가 기능 **정책** 페이지에서 **연결 보안** 옆에 있는 **구성**을 클릭하십시오. 
2. **연결 보안** 페이지의 드롭 다운 목록에서 기본 연결 보안 레벨을 선택하십시오. 여기서 선택하는 값은 사용자 정의 연결 설정을 갖는 디바이스를 제외한 모든 디바이스에 적용됩니다. 이러한 정책은 디바이스가 서버에 연결하는 방법에 영향을 줍니다(실제 디바이스의 설정을 변경하거나 디바이스에 메시지를 전송하지는 않음). 다음 보안 레벨 중 하나를 기본값으로 선택할 수 있습니다. 
    - TLS 선택적
    - TLS와 토큰 인증
    - TLS와 클라이언트 인증서 인증
    - TLS와 토큰 및 클라이언트 인증서 인증

선택하는 보안 레벨을 기반으로 테이블은 영향을 받는 디바이스 수와 설정된 보안 레벨에서의 예측 규제 준수 레벨을 표시합니다. 

3. 필요에 따라 **사용자 정의 연결 추가**를 클릭하여 디바이스 유형 및 사용자 정의 보안 레벨을 선택하십시오. 사용자 정의 보안 설정으로 인한 변경사항을 반영하도록 예측 규제 준수 값이 업데이트됩니다. 
4. **저장**을 클릭하십시오.  

## 블랙리스트 및 화이트리스트 구성

블랙리스트를 사용하여 특정 디바이스의 서버 액세스를 제한하거나 화이트리스트를 사용하여 특정 디바이스에 서버 액세스 권한을 부여합니다. 블랙리스트와 화이트리스트 중 하나만 사용할 수 있고 두 가지를 함께 사용할 수 없습니다. 

### 블랙리스트 구성

1. 위험 및 보안 관리 **정책** 페이지의 **블랙리스트** 섹션에서 **구성**을 클릭하십시오. 
2. **블랙리스트** 페이지에서 **블랙리스트에 추가**를 클릭하십시오. 
3. **블랙리스트에 추가** 창에서 다음 중 하나를 수행하십시오. 
    - **IP 주소/범위** 탭에서 차단하려는 디바이스의 IP 주소 또는 IP 주소 범위(연속된 여러 디바이스의 경우)를 입력하십시오. 
    - **CIDR** 탭에서 CIDR(Classless Inter-Domain Routing) 노테이션이 있는 블록을 입력하십시오. 
    - **국가** 탭에서 모든 디바이스를 차단할 국가를 입력하거나 선택하십시오. 
4. **블랙리스트에 추가** 창에서 **저장**을 클릭하십시오. 
5. 차단된 디바이스 목록을 검토하십시오. IP 주소, CIDR 또는 국가가 목록에 포함된 모든 디바이스는 Watson IoT Platform 서버에 연결할 수 없습니다. 
6. **저장**을 클릭하십시오.

### 화이트리스트 구성
1. 위험 및 보안 관리 **정책** 페이지에서 **화이트리스트** 옆에 있는 **구성**을 클릭하십시오. 
2. **화이트리스트** 페이지에서 **화이트리스트에 추가**를 클릭하십시오. 
3. **화이트리스트에 추가** 창에서 다음 중 하나를 수행하십시오. 
    - **IP 주소/범위** 탭에서 액세스를 허용하려는 디바이스의 IP 주소 또는 IP 주소 범위(연속된 여러 디바이스의 경우)를 입력하십시오. 
    - **CIDR** 탭에서 CIDR(Classless Inter-Domain Routing) 노테이션이 있는 블록을 입력하십시오. 
    - **국가** 탭에서 모든 디바이스의 액세스를 차단할 국가를 입력하거나 선택하십시오. 
4. **화이트리스트에 추가** 창에서 **저장**을 클릭하십시오. 
5. 허용된 디바이스 목록을 검토하십시오. IP 주소, CIDR 또는 국가가 기반으로 목록에 포함된 모든 디바이스는 Watson IoTP Platform 서버에 연결할 수 있습니다. 
6. **저장**을 클릭하십시오.
