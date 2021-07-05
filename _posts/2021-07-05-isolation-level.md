---
title: Isolation Level
tags: SQL JPA Hibernate
aside: false
---

#### 1. 트랜잭션의 이해
#### 2. Isolation Level의 이해

- 아래 쿼리를 이용해서 트랜잭션을 특정 격리 수준으로 시작할 수 있다.
```SQL
USE {데이터베이스명};  
GO  
SET TRANSACTION ISOLATION LEVEL {격리 수준};  
GO  
BEGIN TRANSACTION;  
GO  
SELECT *
FROM {테이블명 A};  
GO  
SELECT *
FROM {테이블명 B}; 
GO  
COMMIT TRANSACTION;  
GO
```