---
title: "첫 글 테스트"
description: "어떻게 글을 작성하고 추가할까요?"
date: 2024-05-10
update: 2024-05-10
tags:
  - 태그입니다
  - 태그2입니다
  - 태그3입니다
series: "첫글 테스트"
---

## 안녕하세요 테스트

테스트테스트테스트테스트테스트테스트

### 안녕하세요

안녕하세요안녕하세요안녕하세요안녕하세요안녕하세요

### 안녕하시렵니까

안녕하세요안녕하세요안녕하세요안녕하세요안녕하세요

## 안녕히가세요 테스트

테스트

### 안녕히가세요

안녕히가세요안녕히가세요안녕히가세요

### 안녕히가세요

안녕히가세요안녕히가세요욥

## 코드 테스트

```typescript
const MiddleSection = () => {
  // 잔디 날짜 계산
  const currentDate = dayjs();
  const currentMonth = currentDate.format('M');
  const nextMonthFirstDay = currentDate.add(1, 'month').startOf('month');
  const currentMonthLastDay = nextMonthFirstDay.subtract(1, 'day');

  const { memberId } = useUser();

  // reward 쿼리
  const { data: reward } = useQuery<RewardPointResponse>({
    queryKey: ['rewardPoint'],
    queryFn: () =>
      API.get(`/member/totalReward/${memberId}`).then(
        response => response.data,
      ),
    initialData: { rewardPoint: 0 }, // 초기 데이터 설정
    enabled: !!memberId, // memberId가 있을 때만 쿼리를 실행
  });
```

## 이미지 테스트

![](bear.png)
