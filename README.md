Ethics in Security (`ethics`)
===============================================================================

This is material for a seminar on ethics in security.  Its focus is on the 
security engineer's role and the ethical problems that might follow.

The module is part of the [Open Security Education][OpenSecEd] project and the 
maintainer is [Daniel Bosk][Maintainer].  The latest release can be found under 
[releases][Releases].  You can safely link directly to the PDFs found there.

[OpenSecEd]: https://github.com/OpenSecEd
[Maintainer]: https://github.com/dbosk
[Releases]: https://github.com/OpenSecEd/ethics/releases


Module Overview
===============================================================================

The module covers ethics in security.  Currently there are the following 
seminars available:

 - `profession` contains the instruction for a seminar where the code of ethics 
   for computer engineering professionals are analysed and discussed in light 
    of actual scenarios.

 - `security-society-seminar` contains the instructions for a seminar which 
   aims to reflect on the role of security, its affect on society and the 
   responsibility of engineers. It uses the codes of ethics of ACM and IEEE as 
   a base for discussing the latter and relies on news and research on the 
   effects on democracy as a base for the former.


File Structure and Building
===============================================================================

*To build* the PDFs, after cloning the repository you must clone its required 
submodules:
```shell
$ git submodule update --recursive --init
```
Then you can go into the directory of the desired document and run `make`.
If you run `make` in the root directory you will recursively transcend the 
directory hierarchy and build everything included in the module.

In each directory the files are structured as follows:

 - <name>.tex contains the main content.
 - aims.tex is an itemized list of the intended learning outcomes, as such it 
   can be included in another document summarizing the list of intended 
   learning outcomes.
 - abstract.tex is an abstract of the lecture, assignment, or similar, and 
   covers the required reading instructions, thus you can include these in 
   a study guide containing all reading instructions for the course.
 - <name>.bib contains the bibliography entries, thus this file can be included 
   along with the reading instructions.

