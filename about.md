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