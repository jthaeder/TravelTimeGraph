# TravelTimeGraph
Travel Time Graph for Directions

Use the google directions api and visualize the output

Only limted uses per day (useage limit of GOOGLE API KEY)

## Installation

### Requirements
* Python 3.x
* jupyter notebook
* [google-maps-services api](https://developers.google.com/maps/documentation/directions/)
    * `$ sudo pip3 install -U googlemaps`
    * Get GOOGLE API KEY, enabled for GOOGLE direction api
    * export key as `GOOGLE_API_KEY`
### Installation TravelTimeGraph
* `$ git clone https://github.com/jthaeder/TravelTimeGraph`
* `$ cd TravelTimeGraph`
* `$ jupyter-notebook`

## Usage
### Launch
Launch `TravelTimeGraph.ipynb`

### Load Methods
`%run ./TravelTimeGraph_Methods.ipynb`

### Edit Route
```
route_tag = {'route_date': '2017-12-04', 
             'route_tag': 'HOME-WORK', 
             'start_point': 'Xstraße 1, 60316 Frankfurt am Main',
             'end_point': 'Xstraße 1, 71034 Böblingen'}
```             

* `route_date`: use yyyy-mm-dd   
* `route_tag`: use '-' for seperating START-END   
* `start_point`, `end_point`: use valid addresses   

### Get Route
One direction only:
`route = getRouteOneDirection(route_tag)`
Both directions
`route, route_back = getRouteBothDirections(route_tag)`
