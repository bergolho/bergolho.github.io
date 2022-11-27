---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: Classes_Cplusplus
title: "Using classes in C++"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: bergolho
# multiple category is not supported
category: Programming
# multiple tag entries are possible
tags: [c++, classes]
# thumbnail image for post
img: ":post_pic3.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2022-11-14 15:38:30 +0900

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-01-01 10:04:30 +0900
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# if you enabled image_viewer_posts you don't need to enable this. This is only if image_viewer_posts = false
#image_viewer_on: true
# if you enabled image_lazy_loader_posts you don't need to enable this. This is only if image_lazy_loader_posts = false
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
#published: false
---

This is an example of how to use classes in C++.

{% highlight cpp %}
// sample_class.cpp
#include <iostream>
#include <string>

using namespace std;

class Foo
{
private:
    int id;
    string name;
public:
    // Constructor initialization
    Foo (int id, string name) : id(id), name(name) { }
    friend ostream& operator<< (ostream& os, const Foo& foo);
};

// Overwrite the print operator
ostream& operator<< (ostream& os, const Foo& foo) 
{  
    os << "Id = " << foo.id << endl;
    os << "Name = " << foo.name << endl;  
    return os;  
}

int main ()
{
    Foo *foo1 = new Foo(1,"Ana");
    Foo *foo2 = new Foo(2,"Beto");
    Foo *foo3 = new Foo(3,"Carla");

    cout << foo1 << endl;
    cout << foo2 << endl;
    cout << foo3 << endl;

    delete foo1;
    delete foo2;
    delete foo3;

    return 0;
}
{% endhighlight %}

Compilation and execution
{% highlight shell %}
$ g++ -o sample_class sample_class.cpp
$ ./sample_class
{% endhighlight %}
