# bildderfrau.de

In this documentation you find the placement details for your Website.  Please find an test-site on the following link:    [Appnexus test site](https://adtechnology.mediaimpact.de/test-appnexus/)

## AdLib

Please use the following JS for the adLib: ```https://acdn.adnxs.com/as/1h/pages/bildderfrau.js```

## Besonderheit 

Superbanner und Billboard haben nur auf der Home getrennte Placements. 

Auf ROS werden die Billboard Sizes über das Superbanner-Placement gecallt. Billboards können trotzdem mit der Size 3x3 gebucht werden


## Placements

 Desktop

| Placement Name|Legacy Format ID (Smart)|Appnexus|
| ------------- |:-------------:| -----:|
|Superbanner|3648|superbanner|
|Sky|3650|sky|
|Billboard|5419|billboard|
|Medium Rectangle|4459|mrec|
|Medium Rectangle 2|4460|mrec_btf|
|Richmedia / Outstream|3651 / 18913|inpage|

 Mobile


| Placement Name|Legacy Format ID (Smart)|Appnexus|
| ------------- |:-------------:| -----:|
|Reminder|12815 (3648)|banner|
|Content Ad|5720 (5419)|mrec|
|Medium Rectangle|4459|mrec_btf|
|Medium Rectangle 2|4460|mrec_btf_2|
|Footer Ad|5721|mrec_btf_3|
|Richmedia / Outstream|6419 (3651) / 29606 (18913)|inpage|

 [Placement Codes](https://github.com/CDPAdSolution/adSolution-Reference/blob/master/publisher-display-reference.md#3-define-the-ad-placements-for-the-website)

# Desktop:

`	adPlacements: ["superbanner","sky","billboard","mrec","mrec_btf","inpage"],`

# Mobile:

`	adPlacements: ["banner","mrec","mrec_btf","mrec_btf_2","mrec_btf_3","inpage"],`
 [Placement Sizes](https://github.com/CDPAdSolution/adSolution-Reference/blob/master/publisher-display-reference.md#4-define-the-sizes-for-every-ad-placement)

# Desktop:

```
	adSlotSizes: {
		"superbanner": [{
			"minWidth": 1,
			"sizes": [[728,90],[728,600],[1000,600]]
		}],
     
		"sky": [{
			"minWidth": 1,
			"sizes": [[160,600],[120,600],[300,600],[500,1000],[1000,1000]]
		}],
     
		"billboard": [{
			"minWidth": 799,
			"sizes": [[800,250]]
		},{
			"minWidth": 969,
			"sizes": [[970,250],[800,250]]
		}],
     
		"mrec": [{
			"minWidth": 1,
			"sizes": [[300,250],[300,600]]
		}],
		
		"mrec_btf": [{
			"minWidth": 1,
			"sizes": [[300,250],[300,600]]
		}],
     
		"inpage": [{
			"minWidth": 1,
			"sizes": [[1,1],[640,360],[1000,300]]
		}],
     
	},
```

# Mobile:

```
	adSlotSizes: {
		"banner": [{
			"minWidth": 1,
			"sizes": [[320,50],[320,75],[320,80]]
		}],
     
		"mrec": [{
			"minWidth": 1,
			"sizes": [[300,250],[320,50],[320,75],[320,160],[300,300]]
		}],
     
		"mrec_btf": [{
			"minWidth": 1,
			"sizes": [[300,250],[320,50],[320,75],[320,160],[300,300]]
		}],
		
		"mrec_btf_2": [{
			"minWidth": 1,
			"sizes": [[300,250],[320,50],[320,75],[320,160],[300,300]]
		}],
		
		"mrec_btf_3": [{
			"minWidth": 1,
			"sizes": [[300,250],[320,50],[320,75],[320,160],[300,300]]
		}],
     
		"inpage": [{
			"minWidth": 1,
			"sizes": [[1,1],[640,360],[1000,300]]
		}],
     
	},
```

# AMP
```
<amp-ad width=320 height=50
        type="appnexus"
        data-target="banner"
        json='{
   "pageOpts":{
      "member":7823
   },
   "adUnits":[

      {
         "disablePsa":true,
         "invCode":"bildderfrau.de-amp-gesundheit_check-banner",
         "sizes":[
            320,
            50
         ],
         "targetId":"banner"
     },
     {
         "disablePsa":true,
         "invCode":"bildderfrau.de-amp-gesundheit_check-mrec",
         "sizes":[
            300,
            250
         ],
         "targetId":"mrec"
     },
      {
         "invCode":"bildderfrau.de-amp-gesundheit_check-banner_sticky",
         "sizes":[
            320,
            50
         ],
         "targetId":"banner_sticky"
      }
   ]
}'>

</amp-ad>


<amp-ad width=300 height=250
        type="appnexus"
        data-target="mrec"
        json='{
   "pageOpts":{
      "member":7823
   },
   "adUnits":[

      {
         "disablePsa":true,
         "invCode":"bildderfrau.de-amp-gesundheit_check-banner",
         "sizes":[
            320,
            50
         ],
         "targetId":"banner"
     },
     {
         "disablePsa":true,
         "invCode":"bildderfrau.de-amp-gesundheit_check-mrec",
         "sizes":[
            300,
            250
         ],
         "targetId":"mrec"
     },
      {
         "invCode":"bildderfrau.de-amp-gesundheit_check-banner_sticky",
         "sizes":[
            320,
            50
         ],
         "targetId":"banner_sticky"
      }
   ]
}'>

</amp-ad>
```
# Sticky Ad
Please ad the following JS
```
<script async custom-element="amp-sticky-ad" src="https://cdn.ampproject.org/v0/amp-sticky-ad-1.0.js"></script>
```
### Please place these Ad container above the fold 

```
<amp-sticky-ad layout="nodisplay">
<amp-ad width=320 height=50
        type="appnexus"
        data-target="banner_sticky"
        json='{
   "pageOpts":{
      "member":7823
   },
   "adUnits":[

      {
         "disablePsa":true,
         "invCode":"bildderfrau.de-amp-gesundheit_check-banner",
         "sizes":[
            320,
            50
         ],
         "targetId":"banner"
     },
     {
         "disablePsa":true,
         "invCode":"bildderfrau.de-amp-gesundheit_check-mrec",
         "sizes":[
            300,
            250
         ],
         "targetId":"mrec"
     },
      {
         "invCode":"bildderfrau.de-amp-gesundheit_check-banner_sticky",
         "sizes":[
            320,
            50
         ],
         "targetId":"banner_sticky"
      }
   ]
}'>

</amp-ad>
</amp-sticky-ad>

```
## Important notes

- For Intext Outstream and for Richmedia we just need one placement with Appnexus.
- __IMPORTANT__ Please palace the "inpage" placement in the required position for InText. Take care that we need the whole website wide for it.

## Help

If you have some question don't hesitate to contact us:


__Timo Nolte__
 
  Head of AdSolutions
  Corporate Digital Platforms

  Tel: +49 30 2591 78009
  Mobile: +49 151 22334646 
  timo.nolte@axelspringer.de


__Carlos Bracho__
 
  Senior Ad Technology Lead 
  Corporate Digital Platforms
  
  Tel: +49 30 2591 76784
  Mobile: +49 151 44619807 
  carlos.bracho@axelspringer.de

__Ad Technology Team__
  adtechnology@axelspringer.de
  
