## dart_documentation_support

The docker image comes from https://cloud.docker.com/repository/docker/timhoar/dart_docs

container to run FORD to generate documentation for DART  
Make sure docker is running - 

~~~
cd /git/DART
docker run -it -v `pwd`:/work timhoar/dart_docs
cd /work/docs
ford ford_config.md
~~~

The best description of options for the FORD config are here:
https://github.com/Fortran-FOSS-Programmers/ford/wiki/Project-File-Options

Also - this container also supports `pandoc` - which can (among other things) convert html to md.

https://pandoc.org/MANUAL.html

The most trivial example would be:

```
pandoc -o bob.md bob.html
```
