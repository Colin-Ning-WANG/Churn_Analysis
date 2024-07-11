#Churn Analysis for Mobile Gaming 玩家流失分析

## Intro 简介
There is no clear definition of churning, and also it's not the reverse of the player retention. The widely accepted explanation for churn is "Players have been inactive for a certain period that they are highly unlikely to return." In real cases, the number here can be very different. 

## Required Fields 需求字段
A database records all the latest states of every player. Or all data including players' behavior across history time. Highly recommend developers record all the players' latest states in one database and keep updated whenever players' info gets renewed.

```PlayerID``` Players Unique Identifier  
```CreateRegion```Account Created Country, only update once  
```AccCreateTime```Account Created Time, only update once  
```LatestLevel```Players' latest level when the last login  
```LastActiveTime```Players' latest login time  
```LastActiveRegion```Players' latest region when the last login  
```LastPayTime```Players' last purchase time  
```LifeTimePay```Players' accumulated payment inside the game  

## Analyze Topics 分析议题
### Churn Players' Level Distribution 玩家流失的关卡分布
1. Clean the data and Select players lastest records.
2. Identify churning players (with time window of 3 or 7 days).
3. Draw the chart of churning players' level distribution.
