---
layout: post
title:  "First pull request ever"
date:   2014-01-01 13:18:08
categories: open source
---

---
layout: post
title:  "My First Pull Request Ever"
date:   2013-12-31 09:25:14
categories: open source
---

I've been coding as a hobbyist for a little while but I've decided to take it more seriously recently, by which I mean, making attempts to contribute to open source projects, as much as I can.  It'll likely mostly be in the area of documentation since I'm not the greatest programmer, however, my first pull request happens to be some actual code for NodeBB, the open sourced node.js based forum by Design Create Play. The problem: NodeBB lets you choose between Mongo or Redis for the backend, however, if you choose Mongo, which doesn't support full-text search in production (at least it's not encouraged), then admins on NodeBB won't be able to create other admin users, since the only way to currently do that is to search for users by username from the /admin/groups folder. Therefore, my pull request adds a 'Make Admin' button on each user's profile button /admin/users, which allows admins to create other admins. 


<a href="https://github.com/designcreateplay/NodeBB/pull/693">First Pull Request Ever</a>
