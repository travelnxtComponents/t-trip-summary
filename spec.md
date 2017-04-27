# t-trip-summary Specification

### Component Use
```javascript

<t-trip-summary data=[[data]] resources=[[resources]] settings=[[settings]]>
</t-trip-summary>

```

### Data
```javascript
{
    "image": "",
    "name": "",
    "location": "",
	"contact": "",
	"distance": "",
	"startDate": [
	              "date": "",
	              "time": ""
	],
	"endDate": [
	               "date": "",
	               "time": ""
	],
	"duration": "",
	"item"[
	{
	      {
	      "passengers": {
		            "adults" : "",
		            "children" : ""
		  },
		  "fareItem": [{
		                     "title": "",
		                     "price": "",
			             "breakup":
				[{
				         "title": "",
					 "price": ""
				}]
		             }]
	}
	}
	],
	
	"total": [
             	            "title": "",
			    "amount": ""
	         ]
	
}
```
### Resources
```javascript

{
    "HideDetailsText": "",
    "showDetailsText": "",
    "distanceTitle": "",
    "startDateTitle": "",
    "endDateTitle": "",
    "durationTitle": "",
    "lessLinkText": "",
    "moreLinkText": "",
    "roomTitle": ""
}
```

### Settings
```javascript

{
      "currency": [
	  "code": "",
	  "format": ""
	  ],
      "minimize": "true",
      "dateFormat": "",
      "timeFormat": "",
      "separator" : ":"
}

```

### Methods
```javascript

collapse() - to hide summary details
expand() - to expand summary 
  
```

### Events
```javascript

t-trip-summary

```

### Listen
```javascript

```


### Styles
```javascript

CSS variable for title text colour (hotel name, room headings)
CSS variable for secondary text colour
CSS variable for link text colour
CSS class for changing map icon
CSS class to change star icons

```

### Info
```javascript

By default all room fares should be shown collapsed
If no fare breakup is provided the fares should not be clickable
No fields are mandatory

```

## Test Cases
- Component should work across all major browsers - Chrome / Mozilla / Safari / Opera / IE etc.
- Verify all exposed public properties are working independently and with complex combination.
- Verify all exposed methods and events are working.

## Steps to Start
- Set Github repository at your end for this project, we will merge them later
- You can use Google/Vaadin's elements (like calender element and textboxes etc.)

## Performance standard
- Any component if opened via [web page tester](https://www.webpagetest.org/), it should load under 500ms (milli seconds).

## Documents
- Visual designs for components - https://projects.invisionapp.com/share/6E9PJ7R4Q#/screens/228211081
- API access : Url - http://demo.travelnxt.com/dev
- Tavisca Elements - https://github.com/atomelements and https://github.com/travelnxtelements
- Vaadin elements - https://vaadin.com/docs/-/part/elements/elements-getting-started.html
- Google - https://elements.polymer-project.org/browse?package=google-web-components
- Tavisca Web component style Guide - https://drive.google.com/open?id=0B7BT_2nBFNYVR2tscE9pRnVJYmc
