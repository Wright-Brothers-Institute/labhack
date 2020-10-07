[![labhack build status](https://travis-ci.org/codefordayton/labhack.svg)](https://travis-ci.org/codefordayton/labhack)

# Air Force Hackathon Website
LabHack, the Air Force Hackathon main website. This is a Jekyll-based website hosted as static files on Github.

## Installation & Usage
    bundle install
    jekyll serve --watch

_Note: Requires Ruby version 1.9.3 =>. For example use [rbenv](https://github.com/sstephenson/rbenv)_   
    
## Publish to Github Pages
Run rake task. **NOTE: It will deploy the generated site to _gh-pages_ branch overwriting it**    
``` 
rake site:publish
```

## Authors
[Code for Dayton](http://codefordayton.org), a [Code for America Brigade](http://www.codeforamerica.org)


## Copyright and license

Modifications to this site are released under the Public Domain.
Original copyright under 2013 Kippt Inc. under [The MIT License ](LICENSE)
