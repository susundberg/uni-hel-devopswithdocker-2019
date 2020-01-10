
# When to use Dockers and what are the benefits

I guess the standard answer is that the dockers provide an way to make scalable and easily deploy-able applications applications/services.

Compared with virtual-machine images - that used to be thing as far as i know - the docker provides little less overhead as the kernel is not "virtualized" but the host kernel is utilized. On the other hand - the fact that same kernel is utilized raises possible security issues at least when speaking from situations where dockers from multiple entities are ran on same machine.

And then there is also Chef - and other tools to automate the installation of packages from known start point.  This provides zero overhead when running and provides excellent isolation (as they are separate HW). But downside is that you cannot utilize your capacity at best possible manner. 

I myself find Dockers usefull for also documenting and testing program building enviroment; in best case you have dockerfile that describes from ubuntu:18.04 what packages you need to compile this project X. And that is verified in CI by doing the build and running the tests. No more word-documents describing the "setup of the development enviroment!" (that are always outdated!).

Example of dockers triumph i think for example web-service-backend - doing something. When the system notices that oh-no -- the load of the existing backend-instances is too high - it will launch more instances. This gets even better when we are at cloud - more servers allocated from farm.

The (00') traditional method of having <N> PC doing the backend/frontend tasks - works, as long as you dont get demand spike. I was witnessing of Lady Gaga tweeting about a service i was part of doing. The servers could not take it. 15min of fame went to "site cannot be reached".  It probably could have been avoided with Dockers and Cloud.

