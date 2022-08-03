
!!! Important
            from django.urls import path
        
            app_name = 'blog'
            urlpatterns = [

            ]
    **Error:** *does not appear to have any patterns in it. If you see valid patterns in the file then the issue is probably caused by a circular import.*

     Make sure you have the above boiler template in your app's `urls.py` when you create your app's `urls.py`. It is important that `urlpatterns` is present or you will get the error when you attempt putting up your development server after adding the blog's app path to the inner project's `urls.py`  .
     