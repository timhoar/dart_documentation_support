## dart_documentation_support

container to run FORD to generate documentation for DART
Make sure docker is running - 

~~~
cd /git/DART
docker run -it -v `pwd`:/work timhoar/dart_docs
cd /work/docs
ford ford_config.md
~~~
