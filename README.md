# Working-with-Django-Rest-Framework


## Django REST framework is a powerful and flexible toolkit for building Web APIs.

### There are six stages for building an API using Django Rest Framework

-  Installing django and django rest framework.
-  creating Models
-  creating Serializers
-  creating views
-  creating urls
-  Our API is ready


## Step by step guide:
- Add 'rest_framework'  in installed apps of settings.py
- Create a new app using 'django-admin startapp app1' and then that app in installed apps of settings.py.
- Create a new Model in models.py and add fields as your needs.
- Now create a new file named serializers.py in app folder and import your model here.
- create a serializer in serializers.py using  Meta data of model:

![image](https://github.com/gaurav0401/Working-with-Django-Rest-Framework/assets/80095859/2b75fc68-1e75-4f0b-9c95-71e123abd727)

- Now import both model and serializer in views.py and create viewset of model:
             ![image](https://github.com/gaurav0401/Working-with-Django-Rest-Framework/assets/80095859/ebc982a2-60e3-4e4d-b5d9-55ac2786e6e9)

- Now in urls.py of app  import  'viewset' here and create a router using routers method of rest_framework
- Now register that router using url  and viewset (i.e router.register(r"url", viewsetname))
             ![image](https://github.com/gaurav0401/Working-with-Django-Rest-Framework/assets/80095859/1ddfa898-e50e-4492-b584-9cb34933b21e)

- Now apply migrations
- Now run server using 'python manage.py runserver' and go to url  which we created for router (i.e /companies  in our case).
   ![image](https://github.com/gaurav0401/Working-with-Django-Rest-Framework/assets/80095859/b08989c2-e1eb-45a2-9a07-f24d56609196)





             



   
