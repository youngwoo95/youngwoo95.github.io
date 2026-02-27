---
title: "ASP.NET Core 정리"
date: 2026-02-28T00:00:00+09:00
draft: false
tags: ["aspnetcore", "dotnet"]
---

## 요약
- ASP.NET Core의 미들웨어 파이프라인 흐름 정리
- DI(의존성 주입) 기본 사용법 정리

## 내용

### 미들웨어 예시
```csharp
app.Use(async (context, next) =>
{
    // before
    await next();
    // after
});



핵심:
- ` ```csharp ` 로 열었으면 **반드시 마지막에 ` ``` ` 로 닫아야 함**
- 이미지는 `static/img/nginx-conf.png`에 업로드했으면 글에서는 **`/img/nginx-conf.png`** 로 참조

---

## ✅ 이미지 문법은 네가 쓴 게 맞아
너가 쓴:

```markdown
![설명](/img/파일명.png)
