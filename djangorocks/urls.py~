from django.conf.urls import patterns, include, url

from django.contrib import admin
admin.autodiscover()

urlpatterns = patterns('',
    (r'^$', 'blog.views.index'),

    url(r'^blog/view/(?P<slug>[^\.]+)/', 
        'blog.views.view_post', 
        name='view_blog_post'),

    url(r'^blog/category/(?P<slug>[^\.]+)/',
        'blog.views.view_category',
        name='view_blog_category'),
    # Examples:
    # url(r'^$', 'djangorocks.views.home', name='home'),
    # url(r'^djangorocks/', include('djangorocks.foo.urls')),

    # Uncomment the admin/doc line below to enable admin documentation:
    # url(r'^admin/doc/', include('django.contrib.admindocs.urls')),

    # Uncomment the next line to enable the admin:
    url(r'^admin/', include(admin.site.urls)),
)
