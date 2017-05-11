# Ginetta home assignment

## Requirements

See [this document](requirements.pdf) (PDF)

## Tasks

- project setup: GitHub repo, GitHub API access
- HTML/CSS/JS skeleton
- API call, re-render
- bold emphasis of matched chars
- line highlighting on hover
- keyboard bindings: up, down, enter
- bonus: proof of modularity: use same search box twice on same page
- bonus: visual pimping

## Notes on the implementation

I chose the "vanilla everything and start from scratch" approach because
1) I think it's the best way to see how I work
2) we rarely get to do this in our daily business
3) time constraints: I don't know any of the nicer current frameworks (React, Angular, Vue) good enough to read documentation _and_ code the solution in 3 hours

In total, I spent around 3.5 hours. The time is mentioned in every commit message. I did not account for the time spent typing this page, and I must have spent another 15-20 minutes looking into things I've never used before. Those would be [HTML imports](https://www.html5rocks.com/en/tutorials/webcomponents/imports/), [HTML templates](https://www.html5rocks.com/en/tutorials/webcomponents/template/) and [Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API). As a bonus, in the 0.5h overtime, I added a [proof of the modularity of my implementation](https://github.com/manofewords/searchbox/commit/757270c3594aafabc619c26d6d35f8af90f6597f) :) 

Up until [this commit](https://github.com/manofewords/searchbox/commit/251037c1d394b686d0f18fe87f21c523f968146b), you could use my implementation via a `file://` URL. If you check out the final result, you will need to run a local server, e.g. `python -m SimpleHTTPServer 8000`. Oh, and the GitHub access token for the API got revoked when I pushed my code. Smart thing GitHub is doing!

## Possible improvements

- implement missing functionality: up/down arrow navigation
- CSS reset, use one of the usual ones
- in real life, I would need to look into browser support, e.g. a [polyfill](https://github.com/github/fetch) for fetch, another one for HTML templates (see [browser support](http://caniuse.com/#feat=template))
- CSS improvement overall: I'm really not used anymore _not_ to use Sass, with nesting, variables, mixins. I wanted to look into [CSS custom properties](https://www.smashingmagazine.com/2017/04/start-using-css-custom-properties/) but didn't have time in the end
