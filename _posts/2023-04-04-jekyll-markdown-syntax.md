---
layout: post
title: jekyll markdown 語法
date: '2023-04-04 03:04:54 +0800'
categories: [其他]
tags: [jekyll]
---
只列一些比較特別的
- [官方文件 - Text and Typography](https://chirpy.cotes.page/posts/text-and-typography/#fnref:footnote)
- [code](https://github.com/cotes2020/jekyll-theme-chirpy/blob/master/_posts/2019-08-08-text-and-typography.md)
## Prompts

> An example showing the `tip` type prompt.
{: .prompt-tip }

> An example showing the `info` type prompt.
{: .prompt-info }

> An example showing the `warning` type prompt.
{: .prompt-warning }

> An example showing the `danger` type prompt.
{: .prompt-danger }
```md
> An example showing the `tip` type prompt.
{: .prompt-tip }

> An example showing the `info` type prompt.
{: .prompt-info }

> An example showing the `warning` type prompt.
{: .prompt-warning }

> An example showing the `danger` type prompt.
{: .prompt-danger }
```

## Tables

| Company                      | Contact          | Country |
|:-----------------------------|:-----------------|--------:|
| Alfreds Futterkiste          | Maria Anders     | Germany |
| Island Trading               | Helen Bennett    | UK      |
| Magazzini Alimentari Riuniti | Giovanni Rovelli | Italy   |

```md
| Company                      | Contact          | Country |
|:-----------------------------|:-----------------|--------:|
| Alfreds Futterkiste          | Maria Anders     | Germany |
| Island Trading               | Helen Bennett    | UK      |
| Magazzini Alimentari Riuniti | Giovanni Rovelli | Italy   |

```

## Links

<http://127.0.0.1:4000>
```md
<http://127.0.0.1:4000>
```

## Code Block Specific filename

```sass
@import
  "colors/light-typography",
  "colors/dark-typography"
```
{: file='_sass/jekyll-theme-chirpy.scss'}
```
### Specific filename
在程式框最後加上
```md
{: file='_sass/jekyll-theme-chirpy.scss'}
```
## Images
```md
![Desktop View](/posts/20190808/mockup.png){: width="972" height="589" }
```
_Full screen width and center alignment_

## Video
`{``%``include embed/youtube.html id='Balreaj8Yqs ``%``}`

