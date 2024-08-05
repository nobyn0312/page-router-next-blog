---
title: '静的生成を使用する場合と静的生成を使用する場合サーバーサイドレンダリング'
date: '2022-01-02'
---

We recommend using **Static Generation** (with and without data) whenever possible because your page can be built once and served by CDN, which makes it much faster than having a server render the page on every request.
ページを一度構築して CDN で提供できるため、リクエストごとにサーバーがページをレンダリングするよりもはるかに高速になるため、可能な限り静的生成

You can use Static Generation for many types of pages, including:
静的生成は、次のような多くの種類のページで使用できます。


- Marketing pages
- Blog posts
- E-commerce product listings
- Help and documentation

-マーケティングページ
-ブログ投稿
-電子商取引の商品リスト
-ヘルプとドキュメント

You should ask yourself: "Can I pre-render this page **ahead** of a user's request?" If the answer is yes, then you should choose Static Generation.

「ユーザーのリクエストに先立ってこのページを事前レンダリングできますか?」と自問する必要があります。答えが「はい」の場合は、静的生成を選択する必要があります。

On the other hand, Static Generation is **not** a good idea if you cannot pre-render a page ahead of a user's request. Maybe your page shows frequently updated data, and the page content changes on every request.

一方、ユーザーのリクエストに先立ってページを事前レンダリングできない場合、静的生成は適していません。ページに頻繁に更新されるデータが表示され、リクエストごとにページ コンテンツが変わる可能性があります。



In that case, you can use **Server-Side Rendering**. It will be slower, but the pre-rendered page will always be up-to-date. Or you can skip pre-rendering and use client-side JavaScript to populate data.

その場合は、サーバーサイドレンダリングを使用できます。速度は遅くなりますが、事前レンダリングされたページは常に最新の状態になります。または、事前レンダリングをスキップし、クライアントサイド JavaScript を使用してデータを入力することもできます。