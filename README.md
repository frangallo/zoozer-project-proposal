# ZooZer

[Heroku link][heroku]

[heroku]: http://www.zoozer.io

## Minimum Viable Product
ZooZer is a clone of Craigslist & Ebay built on Rails and Backbone. Users can:

<!-- This is a Markdown checklist. Use it to keep track of your progress! -->

- [ ] Create accounts
- [ ] Create sessions (log in)
- [ ] Post Items for sale
- [ ] Users can select a radius to see items for sale
- [ ] Bid on an item for sale


## Design Docs
* [View Wireframes][views]
* [DB schema][schema]

[views]: ./docs/views.md
[schema]: ./docs/schema.md

## Implementation Timeline

### Phase 1: User Authentication, Sale Items Creation (~1 day)
I will implement user authentication in Rails based on the practices learned at
App Academy. By the end of this phase, users will be able to create for sale items and offers using a simple text form in a Rails view. The most important part of this phase will be pushing the app to Heroku and ensuring that everything works before moving on
to phase 2.

[Details][phase-one]

### Phase 2: Viewing Sale Items and Offers (~2 days)
I will add API routes to serve sale items and offer data as JSON, then add Backbone
models and collections that fetch data from those routes. By the end of this
phase, users will be able to create sale items and offers, all
inside a single Backbone app.

[Details][phase-two]

### Phase 3: Editing and Displaying SaleItems (~1.5 days)
I plan to use third-party libraries to add functionality to the `SaleItemsForm` and`SaleItemsShow` views in this phase.  I also plan to integrate Filepicker for file upload so users can add images to sale items.

[Details][phase-three]

### Phase 4: Editing and Displaying Offers (~1.5 days)
I plan to use third-party libraries to add functionality to the 'OffersForm', "OffersItem' views in this phase.

[Details][phase-four]

### Phase 5: Searching for Blogs and Posts (~3-4 days)
I'll need to add `search` routes to the SaleItems controllers. On the
Backbone side, there will be a `SearchResultsIndex` composite view that has a 'SearchResultsIndexItem' composite. This composite will include `SalesItemIndex`and `OffersIndex` subviews. These views will use `saleitems` and `offers`collections, but they will fetch from the new `search` routes.

[Details][phase-five]

### Bonus Features (TBD)
- [ ] Search for certain items for sale in given radius
- [ ] User avatars
- [ ] Activity history (e.g. listed items, items bid on)
- [ ] Multiple sessions/session management


[phase-one]: ./docs/phases/phase1.md
[phase-two]: ./docs/phases/phase2.md
[phase-three]: ./docs/phases/phase3.md
[phase-four]: ./docs/phases/phase4.md
[phase-five]: ./docs/phases/phase5.md
