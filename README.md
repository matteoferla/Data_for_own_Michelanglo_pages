# Data for own Michelanglo pages
GitHub at the moment allows Cross-Origin requests for raw files (the changing of the mime type is fine).

## Problem

[Michelanglo](michelanglo.sgc.ox.ac.uk) in order to facilitate the option for users to implement pages locally or offline
(i.e. Zenodo freeze or supplementary data) serves all the various protein used by a page at once if the coordinates are included with the page.

Consequently, it is not feasible to have a Michelanglo page with an inordinate amount of data.
Examples include an endless list of point mutations or docked compounds.

The solution to this is to not use the `type: 'data'` for a protein in its declaration, but a `type: 'url'` (with `value` being the URL with https schema).

Unfortunately, the remote location must be okay with cross-origin requests.

Strangely, `GitHub` is such a place —although it does not allow the serving of HTML pages —as it sets all text files MIME type to `text/plain`.


## Licence

I have no idea about the licence on a PDB file.
I may or may not be the creator of the data. See specific folders for more.
But generally assume no.
