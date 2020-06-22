# Docker
- run application on any operating system given docker includes its own programming language, software packages, databases,...
- No need for virtual environments
- virtual machines are complete copies of a computer system from the operating system on up.
- Virtual environments are used to isolate Python software packages locally. 

# Django for API's
- The most important takeaway is that Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.
- `from rest_framework import generics`
- `class BookAPIView(generics.ListAPIView):`
- A serializer translates data into a format that is easy to consume over the internet, typically JSON, and is displayed at an API endpoint.
- `from rest_framework import serializers`
- We can use the popular cURL program to execute HTTP requests via the command line. All we need for a basic GET request it to specify curl and the URL we want to call.