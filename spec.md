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
