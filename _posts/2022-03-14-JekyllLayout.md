---
title:  "Layout"
excerpt: "(작성중) Layout의 종류"

categories:
  - Blog
tags:
  - [Blog, Jekyll]

toc: true   # table of contents
toc_sticky: true

author_profile: false   # 좌측 프로필 접기(포스트에 들어가면 꺼짐)
sidebar:
  nav: "docs"

date: 2022-03-14
last_modified_at: 2022-03-14
---
# Layout

Layout outer, middle, inner, file.md 적용

# `default`
- 전체 HTML tag를 만드는 가장 바깥의 Layout

# `archive`
- dafault를 Layout으로 갖는 Layout

# `sidebar`
- 메뉴 리스트와 프로필이 나타나는 Layout
- 문서마다 `sidebar.nav` 변수를 수동으로 입력해야함

# `home`
- 최상위 경로의 `/index.html`에서 사용하는 Layout
  
# `Single`
- post의 Layout, 갖는 속성값은 아래와 같다
```
- Header Image: 사이트 전체화면을 관통하는 image와 header를 넣을 수 있음
- Breadcrumb  
- sidebar
- SEO:          title, description, published_date 등 포스트 고유의 <meta> tag가 추가
- title
- content:      post의 내용이 되는 {{ content }} 삽입
- category:     현재 post가 속해있는 category 보여줌
- date:         포스팅 날짜
- share:        포스트를 소셜에서 공유할 수 있게 Link를 제공
- pagination:   목차로 돌아갈 필요 없이 previous/next 버튼 제공
- comment:      댓글 기능
- related post
```

[<cite>Reference</cite> - ExtraBrain 블로그](https://seungwubaek.github.io/blog/mmistake_layout/)
