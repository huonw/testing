testing
=======

Testing github features...

- gh-pages as a submodule/subfolder so that one can autogenerate
  documentation and/or edit the pages while writing code.

  Create the gh-pages branch as usual, then `git submodule -b gh-pages
  {project-url} {directory}`. Now `{directory}` can have gh-pages
  permanently checked out and editable (possibly require a `git config
  push.default current` or something to stop the submodule trying to
  overwrite `master` on each push.)

  The url should be one that you have commit access to, but this 
  obviously breaks other people trying to clone the repo, so there 
  probably has to be some sort of warning for this...
