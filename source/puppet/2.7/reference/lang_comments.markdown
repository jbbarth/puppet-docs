---
layout: default
title: "Language: Comments"
---

Puppet supports two types of comments:

Shell-Style Comments
-----

Shell-style comments (also known as Ruby-style comments) begin with a hash symbol (`#`) and continue to the end of a line. They can start at the beginning of a line or partway through a line that began with code. 

{% highlight ruby %}
    # This is a comment
    file {'/etc/ntp.conf': # This is another comment
      ensure => file,
      owner  => root,
    }
{% endhighlight %}


C-Style Comments
-----

C-style comments are delimited by slashes with inner asterisks. They can span multiple lines. This comment style is less frequently used than shell-style. 

{% highlight ruby %}
    /*
      this is a comment
    */
{% endhighlight %}
