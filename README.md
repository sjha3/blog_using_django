# blog_using_django
Created a simple blog which has an admin <br/>
New posts can be created by admin and added to the blog<br/>
Posts will be displayed on basis of filter applied to 'posts' object in blog/views.py file<br/>
Thus, multiple posts can be displayed dynamically by changing 'posts' object which is passed by view to template<br/>
It is also evident from code that view acts as a bridge between model and template<br/>
"view.py" takes object from model and passes the same to template <br/>
Also, we need to handle the url requests, "mysite/urls.py" sends all "blank" requests (nothing after 127.0.0.1:8000) to "blog.urls" file<br/>
"blog.url" sends all requests to post_list of "views.py" which passed model object 'posts' to template file 'blog/post_list.html'<br/>
This file extracts information from 'post' objects and displays it for url : 127.0.0.1:8000<br/>
