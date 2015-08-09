# Phase 2: Viewing Blogs and Posts

## Rails
### Models

### Controllers
Api::ItemsController (create, destroy, index, show)
Api::OffersController (create, destroy, show, update)

### Views
* blogs/show.json.jbuilder

## Backbone
### Models
* Items (parses nested `offers` association)
* Offers

### Collections
* Items
* Offers

### Views
* ItemForm
* OffersIndex (composite view, contains OffersIndexItem subviews)
* OffersIndexItem
* OfferShow

## Gems/Libraries
