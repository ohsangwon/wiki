# 소프트웨어 마에스트로 8기 과정설명회 후기

### 순서

1. 소마출신 개발자 특강

2. 8기 과정설명

---

## 1. 오픈소스 개발방식의 이해

### `발표자 : 소마3기 KOSS LAB 송태웅`

### 자신이 소마하면서 느낀점

    1. 훌륭한 네트워킹

    2. 시야가 트임(넓어짐)

    3. Coinone 개발자도 소마 3기 동기다. ( 하루 매출 2억 )


### 그 외

    1. 본인은 Linux kernel 속의 성능 측정 도구인 perf 컨트리뷰션을 함

    2. Git을 프로패셔널하게 사용한다.

    *컨트리뷰션 : 풀리퀘스트(Pull Request) 개발 방식 

    *풀리퀘스트 : 다른 사람이 만든 코드에 수정을 제안하는 기능.


### How to develop with Git?

    1. History 관리

    2. 협업 Tool

    3. Commit, Patch


### `*커밋 단위로 개발하라`

    Hello World를 찍을 때 Git이 필요하다? 아니다?

     ==> 오픈소스 프로젝트에는 필요하다!

### Git과 GitHub의 차이

    Git은 가벼운 GitHub이다.

    remote 정도 기능만 한다. ( read only? )


[OpenHub](https://www.openhub.net/) : 어떤 오픈소스가 있는지 보러가보자

### ~~리눅스 커널 개발과정 ( 스킵하심 )~~

### utfrace 간단한 소개

[링크](https://github.com/namhyung/uftrace) : Function (graph) tracer for user-space

    C, C++ 트레이싱 하는 오픈소스 라이브러리

`예제`

```
$ cat hello.c
#include <stdio.h>
int main(void)
{
   return printf("%s world\n", "Hello");
}

$ gcc -pg -o hello hello.c

$ uftrace ./hello
Hello world
# DURATION    TID     FUNCTION
            [ 7516] | main() {
 414.023 us [ 7516] |   printf();
 697.310 us [ 7516] | } /* main */
```

    Pull Request, Review -> Code Style등 가이드라인 정리


### 커밋 단위

    커밋을 너무 길게 하는 걸까? 
    
    아님 너무 짧은걸까?

    ...

    사실 작은게 좋다고 한다. 

    함수도 함수명과 내용이 한번에 이해 가능하게 만드는게 좋듯이

    하나의 목적에 맞게 만들어라.

---

## 2. 8기 과정소개

### `발표자 : 정보통신기술지능센터 OOO님 (이름을 못들음..)`

### 소프트웨어 마에스트로 소개

    소프트웨어 마에스트로는 미래창조과학부에서 운영하는 과정으로 국내 소프트웨어 전문가들을 만들자는 취지하에 운영되고 있다. 
    
    소프트웨어 산업 분야별 전문가를 멘토로 지정하여 도제식 교육방식을 통해 단계별 프로젝트를 수행하며서 지도받는 시스템이다.

### 소마 인재상

    * 지능정보사회 중장기 종합대책
    
    * 글로벌 수준의 지능정보기술
 
    * 창의적이고 혁신적인 인재

    (즉, 창조적 문제해결 역량과 협업에 익숙한 융합형 인재를 뽑겠다는 말)

### SW에 대한 자신의 꿈을 펼치는 새로운 도전의 기회
    
    1. SW 최우수 인재 육성

    2. 최고 전문가의 실전형 프로젝트 교육

    3. 체계적이고 파격적인 지원 시스템

    * 약 5개월 교육

    * 8기에선 최고 10인 인증금 -> 해외교육(연수)로 바뀜

### 양방향 교육

    프로젝트 중심 융합 인력 교육 실시

    N : N 멘토링 강화 
    ( 저번 까지만해도 N : 1 멘토링이라 멘토에 따라 팀성적이 갈린다고 함 )

    기술, 사업, 창의성 몰입형 교육 실시
    ( 발표자분은 24시간 연수센터에서 공부해도 된다고함 ㅎㅎ; )

    100명 선발 -> 5개월 교육 -> 10명 선발 -> 2개월 해외연수

### 교육 일정

|         | 8월 | 9월 | 10월 | 11월 | 12월 |
|:-------:|:---:|:---:|:---:|:----:|:----:| 
| 기본교육 | 알고리즘 교육 | 알고리즘 교육 | 알고리즘 교육 | 알고리즘 교육 | 알고리즘 교육 |
| 기술교육 | 프로젝트개발 방법론 | IOT, Clude | Big Data, Mobile | 기업가 정신 (BM관련) | PT | 
| 프로젝트 | 팀빌딩 | 멘토링 기반 | 멘토링 기반 | 멘토링 기반 | 멘토링 기반 |
| 평가     | 프로젝트 심의 | 기술교육 과제 평가 (2주) |  기술교육 과제 평가 (2주)
|||                        |중간평가 |     | 결과평가 |

### 특전

    - SW개발병

    - 특허 창업 비용

    - 멘토링 (51명의 멘토)

    - 개발 공간 (24시간)

    - 지원금

    - 프로젝트 개발비

    - IT 기기

    - 글로벌 SW교육

    - 사후 지원 (네트워킹 등...)

### 지원 시 유의사항

    * 200명 서류 합격 (2배수) --> ( 코딩테스트, 인적성, 면접 ) --> 100명 최종 합격
    
    * 서류 심사 시 중요한 것 (순서대로)

    1. SW 개발 이력 등

    2. 비전 / 열정

    3. 인적 소양

### 기술교육 (9월 ~ 10월)

    * IOT, Cloude, Big Data, Mobile (최신 트렌드 기술)

    진짜 제대로된 교육을 한다고 한다.
    
    밑바닦까지 배우고 실습하고 과제하면서 교육시킨다고 한다.

    소마 출신이라면 CEO나 기타등등 훌륭한 위치에 올라갈 것이라 다양한 교육기회를 준다.

    하나만 보고 하지말라는 취지라고 한다.

### 제일 중요

    이력서 엄청 잘써야 한다.

    서류합격 200명인데, 평균 900 ~ 1000명 정도 지원한다고 한다.

    서류검토만 전문적으로 하는 전문가가 50 ~ 100명이다.

    이들이 서류내용을 꼼꼼히 읽을것이라고 한다.

### 개발 능력

    수상경력 - 가산점 정도 생각한다.

    역량이 있는지에 대한 걸 어필하면 좋다고 한다.

### 코딩테스트

    문제해결능력을 보는데, 난이도는 장담을 못하겠지만

    너무 어렵게 나오는건 아니라고한다.

    테스트때 못풀어도 면접때 왜 이렇게 코딩했는지 설명하는 시간이 있음.

### 면접때 프로젝트 시연

    필요하면 노트북을 가져와서 프로젝트 시연해도 됨