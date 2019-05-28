---
title : "关于Yuhari的一些资料"
description: "我是**Yuhari**，是该博客的作者，请容许我花费些文字来介绍下自己，也许这样你能了解我，并知晓这个站点上的文字是否适合你来阅读。"
slug: "who"
tags: ["about"]
minute: 3
date: 2019-05-27T15:35:51-05:00
related: ["/about/about1", "/about/about2"]

---

### 写在前面
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;我是**Yuhari**，是该博客的作者，请容许我花费些文字来介绍下自己，也许这样你能了解我，并知晓这个站点上的文字是否适合你来阅读。

---

### 正文

```go
// 教育经历
type University struct {
	Name           string
	GraduationDate string
}

// 个人信息
type Personal struct {
	Name      string
	BirthDate string
	Age       int
	Married   bool
	Address   string
}

// 个人爱好
type Hobby string

// 技能偏好
type Skill string

// yuhari
type Yuhari struct {
	Personal *Personal
	EduExp   []University
	Hobbies  []Hobby
	Skills   []Skill
}

func New() *Yuhari {
	yuhari := new(Yuhari)

	yuhari.Personal = &Personal{
		Name:      "Yuhari",
		BirthDate: "1992-03-25",
		Age:       27,
		Married:   false,
		Address:   "Nanjing, China",
	}

	yuhari.EduExp = []University{
		University{
			Name:           "WHU",
			GraduationDate: "2014-07-10",
		},
	}

	yuhari.Hobbies = []Hobby{
		"电影", "摄影", "写代码", "ACG", "历史文化","时政",
	}

	yuhari.Skills = []Skill{
		"熟悉后端开发的多种编程语言", "熟悉Linux、windows等开发环境", "熟悉服务器运维相关", "熟悉软件开发流程",
	}

	return yuhari
}
```
---

### 结语
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;请原谅我突兀地用这样一个代码段来介绍自己，实际上确实是在想要介绍自己时，突然不清楚如何很好地组织语言了（*理工男在这方面确实会迷茫*）。不过，也许通过这样的形式了解**Yuhari**更合适也说不定。