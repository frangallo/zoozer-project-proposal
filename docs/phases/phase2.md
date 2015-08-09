# Phase 2: Viewing Blogs and Posts

## Rails
### Models

### Controllers
Api::SellItemsController (create, destroy, update, show)
Api::OffersController (create, destroy, show, index)

### Views
* items/offers.json.jbuilder

## Backbone
### Models
* SellItems (parses nested `offers` association)
* Offers

### Collections
* SellItems
* Offers

### Views
* SellItemsShow
* SellItemsForm
* OffersForm
* OffersIndex (composite view, contains OffersIndexItem subviews)
* OffersIndexItem

## Gems/Libraries
