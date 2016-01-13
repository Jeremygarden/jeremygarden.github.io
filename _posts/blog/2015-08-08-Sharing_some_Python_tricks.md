---
layout: post
title: "Sharing some Python Trick"
author: me
excerpt: "Useful tips that were found when wrote Python"
categories: blog
tags: [Coding, Python, Note]
modified:
image:
  feature: mushroom.jpg
  <!-- credit: WeGraphics -->
  <!-- creditlink: http://wegraphics.net/downloads/free-ultimate-blurred-background-pack/ -->
share: true
comments: true
---




1.How to easily get the index & value from sequences

{% highlight python %}
my_list = [5,2,3,7,9,1,0,3,8]
   for i,ele in enumerate(my_list):
       print "index",i,"element",ele;

   for i,ele in enumerate(li[::-1]);
       print "index",i, "element", ele

#dic is different

my_dic = {'emp_id':'007','emp_name': 'coop', 'city':'bos'}
   for i, ele in my_dic.iteritems():
	   print i, ":", ele



{% endhighlight %}


2.Differences among deleting elements from list

* del: according to the given index without returning the values.
* pop: according to the given index with returning the values, otherwise directly wipe out the last element and return its value.
* remove: according the value of the elements with returning None.



3.(Easier way)counting in the sequence 

What if I have to count out the duplicates from the sequence?

The common code might be:


{% highlight python %}

def get_counts(sequence):    
    counts = {}
    for x in sequence:
        if x in counts:
            counts[x] += 1
        else:
            counts[x] = 1
    return counts

def top_counts(counts,n=10):   
    value_key_pairs = [(number, name) for name, number in counts.items()]
    value_key_pairs.sort()
    return value_key_pairs[-n:]

{% endhighlight %}

There is a class called collections.Counter in Python Collections Library which can definitely simplify the code: 
{% highlight python %}
from collections import Counter

counts = Counter(sequence)
counts.most_common(15)

{% endhighlight %}


More is on the way....
Record my faults and results for help others.


Jeremy



