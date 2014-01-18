---
layout: page
permalink: /about/
title: 
tags: [Jekyll, about, ruby, self introduction]
image:
  feature: about.jpg
  credit: stonehenge by Haisu
  creditlink: http://lofter.zuohaisu.cn/post/c1f2d_19938a
share: false
---

*Your life can be what you want it to be 你能够主宰你的自己的生活*

## About Me 自我介绍

I has been working in the Internet industry since 2011. Before the role of Product Manager at [Qvod Technology](http://www.qvod.com/), I acquired a MSc in Entreprenuership and Innovation Management at [KTH Royal Institution of Technology](http://www.kth.se/), Stockholm and a BSc in Applied Psychology at [Zhejiang University](http://www.zju.edu.cn/). Besides, I worked as Project Manager with [SXL Group](http://www.sxlgroup.com/) in Shanghai for one year.

My crossover background between art, science, business and technology make me easy to cut into any industry thru different mindsets. My passion is to improve the daily life of human being with innovative solution and service. I initiated the hacker-style self-development in the end of 2013, after I realized my personality was not social-oritented even though I held a few social skills. I enjoy the status of focusing on complex issue and are willing to share the results with others.

{% highlight ruby linenos %}
#Self.introduce
def introduce
  @me = Self.new
  @me.name = "Haisu Zuo"
  @me.age = "Since 1987"
  @me.employed_by = "Qvod Technology"
  @me.location = "Shenzhen"
  @me.status = "In a relationship"
  if @me.save
    redirect_to /index/
  else
    render /about/
  end
end
{% endhighlight %}