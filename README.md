# spring-gift-enhancement
# 1단계 - 상품 카테고리

## 요구사항
### 기능 요구사항
상품 정보에 카테고리를 추가한다. 상품과 카테고리 모델 간의 관계를 고려하여 설계하고 구현한다.

- 상품에는 항상 하나의 카테고리가 있어야 한다.
- 상품 카테고리는 수정할 수 있다.
- 관리자 화면에서 상품을 추가할 때 카테고리를 지정할 수 있다.
- 카테고리는 1차 카테고리만 있으며 2차 카테고리는 고려하지 않는다.
- 카테고리의 예시는 아래와 같다.
- 교환권, 상품권, 뷰티, 패션, 식품, 리빙/도서, 레저/스포츠, 아티스트/캐릭터, 유아동/반려, 디지털/가전, 카카오프렌즈, 트렌드 선물, 백화점, ...

### 프로그래밍 요구사항
프로그래밍 요구 사항
구현한 기능에 대해 적절한 테스트 전략을 생각하고 작성한다.
- Repository 계층을 작성했으니 Service 계층 테스트도 작성해본다.

# 2단계 - 상품 옵션

## 요구사항
### 기능 요구사항
상품 정보에 옵션을 추가한다. 상품과 옵션 모델 간의 관계를 고려하여 설계하고 구현한다.

- 상품에는 항상 하나 이상의 옵션이 있어야 한다.
- 옵션 이름은 공백을 포함하여 최대 50자까지 입력할 수 있다.
- 특수 문자
  - 가능: ( ), [ ], +, -, &, /, _ 
  - 그 외 특수 문자 사용 불가
  - 옵션 수량은 최소 1개 이상 1억 개 미만이다.
  - 중복된 옵션은 구매 시 고객에게 불편을 줄 수 있다. 동일한 상품 내의 옵션 이름은 중복될 수 없다.

# 3단계 - 옵션 수량 차감

## 요구사항
### 기능 요구사항
상품 옵션의 수량을 지정된 숫자만큼 빼는 기능을 구현한다.
- 별도의 HTTP API를 만들 필요는 없다.
- 서비스 클래스 또는 엔티티 클래스에서 기능을 구현하고 나중에 사용할 수 있도록 한다.

### 프로그래밍 요구사항
구현한 기능에 대해 적절한 테스트 전략을 생각하고 작성한다.