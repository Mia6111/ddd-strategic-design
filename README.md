# 키친포스

## 요구 사항

- 포스 시스템을 구현한다

- 메뉴
  - [ ] 메뉴는 이름과 가격을 갖는다.
  - [ ] 메뉴는 0원 이상의 가격을 가져야 한다 
  - [ ] 메뉴는 판매할 상품 목록을 갖는다 
  - [ ] 메뉴는 유효한 메뉴 그룹에 속해야 한다
  - [ ] 메뉴를 생성할 수 있다
    - [ ] 이 때, 메뉴의 가격은 판매할 상품 목록의 개별 (수량 * 가격)의 총합보다 같거나 커야 한다
  - [ ] 전체 메뉴를 조회할 수 있다
- [ ] 메뉴 그룹
  - [ ] 메뉴 그룹은 이름을 갖는다
  - [ ] 메뉴 그룹을 생성할 수 있다
  - [ ] 전체 메뉴 그룹을 조회할 수 있다
- 주문 테이블
  - [ ] 주문 테이블은 손님 수와 점유 상태를 갖는다
  - [ ] 주문 테이블은 유효한 테이블 그룹에 속해야 한다
  - [ ] 주문 테이블을 생성할 수 있다
  - [ ] 전체 주문 테이블을 조회할 수 있다
  - [ ] 특정 주문 테이블의 점유 상태를 변경할 수 있다
    - [ ] 이 때, 해당 주문테이블에 "요리중"이거나 "식사중"인 주문이 있어서는 안된다
  - [ ] 특정 주문 테이블의 손님 수를 조회할 수 있다 
  - [ ] 특정 주문 테이블의 손님 수를 변경할 수 있다
    - [ ] 이 때, 손님 수는 0명 이상이여야 한다
- 테이블 그룹
  - [ ] 테이블 그룹은 생성 시각을 갖는다
  - [ ] 테이블 그룹은 1개 이상의 주문 테이블 목록을 포함한다
  - [ ] 테이블 그룹을 생성할 수 있다
    - [ ] 이 때, 포함할 주문 테이블은 점유된 (채워) 상태여야 하고 
      속한 테이블 그룹이 없어야 한다
  - [ ] 특정 테이블 그룹을 삭제할 수 있다
    - [ ] 이 때, 주문테이블ID가 가장 작은 주문테이블이 있어야 하고,  
      해당 주문테이블에 "요리중"이거나 "식사중"인 주문이 있어서는 안된다
- 주문
  - [ ] 주문은 주문시각과 주문 상태를 갖는다
    - [ ] 주문 상태는 "요리중", "식사중","완료" 중 하나이다
  - [ ] 주문은 유효한 주문 테이블에 속해야 한다
  - [ ] 주문은 1개 이상의 주문 아이템 목록을 포함한다
  - [ ] 주문을 생성할 수 있다
    - [ ] 이 때, 포함할 주문아이템이 1개 이상이어야 한다
      유효한 주문테이블에 속해야 한다
    - [ ] 생성된 주문은 주문 테이블을 갖는다
      - [ ] 해당 주문테이블이 이미 테이블 그룹에 속한 경우, 
        생성될 주문은 해당 테이블 그룹의 주문 테이블 중 주문테이블ID가 가장 작은 주문테이블을 갖게 된다
      - [ ] 해당 주문테이블이 아직 테이블 그룹에 속하지 않은 경우, 
        생성될 주문은 해당 주문 테이블을 갖게 된다
    - [ ] 생성된 주문은 "요리중" 상태이다
  - [ ] 전체 주문을 조회할 수 있다
  - [ ] 특정 주문의 상태를 변경할 수 있다
    - [ ] 이 때, 해당 주문의 현재 상태는 "완료"가 아니여야 한다
- 주문아이템
  - [ ] 주문아이템은 순서를 갖는다
  - [ ] 주문아이템은 유효한 주문에 속해야 한다
  - [ ] 주문아이템은 메뉴와 개별 메뉴에 대한 주문 수량을 가진다 
    - [ ] 주문수량에 대한 체크가 없다?
  - [ ] 주문 아이템은 주문 생성시 같이 생성된다
- 상품
  - [ ] 상품은 이름과 가격을 갖는다
  - [ ] 상품을 생성할 수 있다
    - [ ] 이 때, 상품의 가격은 0원 이상이여야 한다
  - [ ] 전체 상품 목록을 조회할 수 있다

- 

## 용어 사전

| 한글명 | 영문명 | 설명 |
| --- | --- | --- |

## 모델링

- 
