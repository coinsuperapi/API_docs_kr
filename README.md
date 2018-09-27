# REST API

소개

```
Exchange api는 무역센터에서 외부 개발자를 상대하여 제공하는 개발 인터페이스이다.
```

------

업그레이드 기록

| 버전        | 시간       | 설명                         | 작가     |
| --------- | -------- | -------------------------- | ------ |
| v1.0.1(R) | 20180626 | 인터페이스를 증가하다:무역목록을 사용할수 있다. | liyong |

------

## [1、**전면규칙**](https://github.com/coinsuperapi/API_docs_kr/wiki#1%EC%A0%84%EB%A9%B4%EA%B7%9C%EC%B9%99)

#### [인터페이스 방문 접두사](https://github.com/coinsuperapi/API_docs_kr/wiki#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4-%EB%B0%A9%EB%AC%B8-%EC%A0%91%EB%91%90%EC%82%AC)

#### [인터페이스 규칙](https://github.com/coinsuperapi/API_docs_kr/wiki#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4-%EA%B7%9C%EC%B9%99)

##### [전면 데이터 격식 정의](https://github.com/coinsuperapi/API_docs_kr/wiki#%EC%A0%84%EB%A9%B4-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EA%B2%A9%EC%8B%9D-%EC%A0%95%EC%9D%98)

##### [서명묘사](https://github.com/coinsuperapi/API_docs_kr/wiki#%EC%84%9C%EB%AA%85%EB%AC%98%EC%82%AC) 

#####  [서명 생성 방법 실례](https://github.com/coinsuperapi/API_docs_kr/wiki#%EC%84%9C%EB%AA%85-%EC%83%9D%EC%84%B1-%EB%B0%A9%EB%B2%95-%EC%8B%A4%EB%A1%80) 

####  [전면 통용 상태 코드](https://github.com/coinsuperapi/API_docs_kr/wiki#%EC%A0%84%EB%A9%B4-%ED%86%B5%EC%9A%A9-%EC%83%81%ED%83%9C-%EC%BD%94%EB%93%9C) 

------

## [2、상세 인터페이스 정의](https://github.com/coinsuperapi/API_docs_kr/wiki#2%EC%83%81%EC%84%B8-%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4-%EC%A0%95%EC%9D%98)

### [인터페이스 목록](https://github.com/coinsuperapi/API_docs_kr/wiki#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4-%EB%AA%A9%EB%A1%9D)

### [API인터페이스 정의](https://github.com/coinsuperapi/API_docs_kr/wiki#api%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4-%EC%A0%95%EC%9D%98)

#### [1.사용자 자산 조회 관리](https://github.com/coinsuperapi/API_docs_kr/wiki#1%EC%82%AC%EC%9A%A9%EC%9E%90-%EC%9E%90%EC%82%B0-%EC%A1%B0%ED%9A%8C-%EA%B4%80%EB%A6%AC)

##### [1.1 개인 자산정보 획득](https://github.com/coinsuperapi/API_docs_kr/wiki#11-%EA%B0%9C%EC%9D%B8-%EC%9E%90%EC%82%B0%EC%A0%95%EB%B3%B4-%ED%9A%8D%EB%93%9D)

#### [2.의뢰와 거래](https://github.com/coinsuperapi/API_docs_kr/wiki#2%EC%9D%98%EB%A2%B0%EC%99%80-%EA%B1%B0%EB%9E%98)

##### [2.1 의뢰를 사다](https://github.com/coinsuperapi/API_docs_kr/wiki#21-%EC%9D%98%EB%A2%B0%EB%A5%BC-%EC%82%AC%EB%8B%A4)

##### [2.2 의뢰를 팔다](https://github.com/coinsuperapi/API_docs_kr/wiki#22-%EC%9D%98%EB%A2%B0%EB%A5%BC-%ED%8C%94%EB%8B%A4)

##### [2.3 의뢰 취소](https://github.com/coinsuperapi/API_docs_kr/wiki#23-%EC%9D%98%EB%A2%B0-%EC%B7%A8%EC%86%8C)

##### [2.4 의뢰증서 상태 조회(의뢰번호에 근거하여)](https://github.com/coinsuperapi/API_docs_kr/wiki#24-%EC%9D%98%EB%A2%B0%EC%A6%9D%EC%84%9C-%EC%83%81%ED%83%9C-%EC%A1%B0%ED%9A%8C%EC%9D%98%EB%A2%B0%EB%B2%88%ED%98%B8%EC%97%90-%EA%B7%BC%EA%B1%B0%ED%95%98%)

##### [2.5 주문 거래 상세 정보 조회(의뢰 번호에 근거하여)](https://github.com/coinsuperapi/API_docs_kr/wiki#25-%EC%A3%BC%EB%AC%B8-%EA%B1%B0%EB%9E%98-%EC%83%81%EC%84%B8-%EC%A0%95%EB%B3%B4-%EC%A1%B0%ED%9A%8C%EC%9D%98%EB%A2%B0-%EB%B2%88%ED%98%B8%EC%97%90-%EA%B7%)

##### [2.6 오더번호 목록(개인이 완전히 거래 성사하지 못한 의뢰 증서 목록)](https://github.com/coinsuperapi/API_docs_kr/wiki#26-%EC%98%A4%EB%8D%94%EB%B2%88%ED%98%B8-%EB%AA%A9%EB%A1%9D%EA%B0%9C%EC%9D%B8%EC%9D%B4-%EC%99%84%EC%A0%84%ED%9E%88-%EA%B1%B0%EB%9E%98-%EC%84%B1%EC%82%AC)

#### [3.시세](https://github.com/coinsuperapi/API_docs_kr/wiki#3%EC%8B%9C%EC%84%B8)

##### [3.1 깊이 시세(최신 깊이도 데이터)](https://github.com/coinsuperapi/API_docs_kr/wiki#31-%EA%B9%8A%EC%9D%B4-%EC%8B%9C%EC%84%B8%EC%B5%9C%EC%8B%A0-%EA%B9%8A%EC%9D%B4%EB%8F%84-%EB%8D%B0%EC%9D%B4%ED%84%B0)

##### [3.2 가격시세(최신 주문서 데이터)](https://github.com/coinsuperapi/API_docs_kr/wiki#32-%EA%B0%80%EA%B2%A9%EC%8B%9C%EC%84%B8%EC%B5%9C%EC%8B%A0-%EC%A3%BC%EB%AC%B8%EC%84%9C-%EB%8D%B0%EC%9D%B4%ED%84%B0)

##### [3.3 시간대 시세(최신 k라인 데이터)](https://github.com/coinsuperapi/API_docs_kr/wiki#33-%EC%8B%9C%EA%B0%84%EB%8C%80-%EC%8B%9C%EC%84%B8%EC%B5%9C%EC%8B%A0-k%EB%9D%BC%EC%9D%B8-%EB%8D%B0%EC%9D%B4%ED%84%B0)

##### [3.4 실시간 거래 성사 시세(최신 거래 성사 시세 데이터)](https://github.com/coinsuperapi/API_docs_kr/wiki#34-%EC%8B%A4%EC%8B%9C%EA%B0%84-%EA%B1%B0%EB%9E%98-%EC%84%B1%EC%82%AC-%EC%8B%9C%EC%84%B8%EC%B5%9C%EC%8B%A0-%EA%B1%B0%EB%9E%98-%EC%84%B1%EC%82%AC-%EC%8B%)

##### [3.5 거래가능한 거래쌍 목록](https://github.com/coinsuperapi/API_docs_kr/wiki#35-%EA%B1%B0%EB%9E%98%EA%B0%80%EB%8A%A5%ED%95%9C-%EA%B1%B0%EB%9E%98%EC%8C%8D-%EB%AA%A9%EB%A1%9D)

## 저희를 연락하십시오

```
도움이 필요하시면 아래의 api문제교류 동아리를 가입하세요(가입시 비고란에 api+coinsuper아이디를 입력하세요)：
1.QQ동아리：472488338 
2.Telegram 전문 동아리：https://t.me/joinchat/HEgiSxBKVx6nwQ33otJ3Zg
```

