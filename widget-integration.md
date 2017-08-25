# Stickee Widget

## What we offer

Stickee can provide content units for various products, sizes and styles depending
on your requirements.

We offer content units providing both broadband and mobile phone comparison.

Adding a widget to your site takes just a snippet of HTML and JS code.

## What it looks like

### Broadband
[Broadband demo 1](http://example.stickeebroadband.co.uk/?widget=full)
[Broadband demo 2](http://example.stickeebroadband.co.uk/?widget=mini)

### Mobiles
[Mobiles demo 1](http://example.stickeebroadband.co.uk/?widget=mini)
[Mobiles demo 2](http://example.stickeebroadband.co.uk/?widget=mini)

The content units are fully responsive, and can be inserted into any page within any
sized container.

## Installation

## JS Script

On the page or template you want the widget to appear add the following code to the <head> section of the page:

```<script src="//stickee-comparison.s3-eu-west-1.amazonaws.com/widget/stickee-comparison-widget-min.js" async></script>```

This JS snippet only needs to be added once if you are taking both a mobiles and broadband widget.

## HTML Placeholder

The script will look for a HTML element with the class .stickee-comparison-widget and replace this with the widget. The HTML element contains parameters that define the behaviour of the widget. Please note, the params provided are all required.

### Broadband

Please insert the following placeholder element in the page or template where you would like the widget to appear:

```
<div class="stickee-comparison-widget"
    data-sector="broadband"
    data-partner="stickee"
    data-type="mini"
    data-width="500">
</div>
```


You can change the data-width parameter to suit the layout of your page- this can also be a percentage if required. The widget's height will change dynamically based on the content served. It is recommended that you don’t apply a fixed width unless required.

There are two options for 'data-type': "full" or "mini." Mini reveals the postcode checker initially, then once a postcode has been entered, the results are displayed below.



### Mobiles

Please insert the following placeholder element in the page or template where you would like the widget to appear:

```
<div class="stickee-comparison-widget"
    data-sector="mobiles"
    data-partner="stickee"
    data-type="mini-5"
    data-width="500">
</div>
```


You can change the data-width parameter to suit the layout of your page- this can also be a percentage if required. The widget's height will change dynamically based on the content served. It is recommended that you don’t apply a fixed width unless required.

There are two options for 'data-type': "full" or "mini." Mini allows you to choose how many deals your widget displays by default on page load, for example “Mini-5” will display 5 deals, whist “Mini-1” will display 1 deal. 

## Pre-filtering deals

## Broadband

The following HTML snippets can be used to pre-filter broadband widgets. Please remember to replace <data-partner> to your partner ID.:

### Broadband Only

```
<div class="stickee-comparison-widget"
   data-sector="broadband"
   data-partner="stickee"
   data-type="mini"
   data-width="500"
   data-filters=”filters[dealtype]=broadband”>
</div>
```

### Broadband and Phone

```
<div class="stickee-comparison-widget"
   data-sector="broadband"
   data-partner="stickee"
   data-type="mini"
   data-width="500"
   data-filters=”filters[dealtype]=broadband-phone”>
</div>
```


### Broadband, Phone and TV

```
<div class="stickee-comparison-widget"
   data-sector="broadband"
   data-partner="stickee"
   data-type="mini"
   data-width="500"
   data-filters=”filters[dealtype]=broadband-phone-tv”>
</div>
```

### Providers

For providers, use the following code:

```
<div class="stickee-comparison-widget"
   data-sector="broadband"
   data-partner="stickee"
   data-type="mini"
   data-width="500"
   data-filters=”filters[suppliers][]=supplierID”>
</div>
```


|---------------|------------|----------------------|------------|
| BT            | ba3lLMM2yA | First Utility        | eyxlnJmlNP |
| Virgin Media  | OBxpm3Zl97 | John Lewis Broadband | WPXpDwR2DN |
| Plusnet       | Zy1j09olB8 | Now TV               | zGe2GRylMb |
| Sky           | eDnjZ9VpAr | Origin Broadband     | WyPloLA2zL |
| TalkTalk      | LwKpE0x25E | Post Office          | VE6jk6bpBr |
| EE            | eDnjZVVjAr | SSE                  | 8ryp8nxl0x |
| Direct Save   | QvV2OQPjGD | Vodafone             | KNvj4MPlX4 |


## Mobiles

### Makes

The following HTML snippet can be used to pre-filter mobiles widgets based on makes. Please remember to replace <data-partner> to your partner ID.:

```
<div class="stickee-comparison-widget"
   data-sector="mobiles"
   data-partner="stickee"
   data-type="mini"
   data-width="500"
   data-filters=”filters[make]=makeID”>
</div>
```


Alcatel | 22 | Kodak | 62
Amazon | 61 | LG | 6
Apple | 19 | Lenovo | 40
BlackBerry | 2 | Motorola | 1
Caterpillar | 56 | Nokia | 4
Dewalt | 68 | Samsung | 5
Doro | 42 | Sony | 54
Google | 15 | Vodafone | 26
HP | 35 | WileyFox | 66
HTC | 13 | ZTE | 8
Huawei | 12 | 

### Models

The following HTML snippet can be used to pre-filter mobiles widgets based on makes and models. Please remember to replace <data-partner> to your partner ID.:

```
<div class="stickee-comparison-widget"
   data-sector="mobiles"
   data-partner="stickee"
   data-type="mini"
   data-width="500"
   data-filters=”filters[make]=makeID”&filters[model]=modelID”>
</div>
```

A full list of available models can be downloaded here. 

### Networks

The following HTML snippet can be used to pre-filter mobiles widgets based on networks. Please remember to replace <data-partner> to your partner ID.:

```
<div class="stickee-comparison-widget"
   data-sector="mobiles"
   data-partner="stickee"
   data-type="mini"
   data-width="500"
   data-filters=”filters[networks]=networkID”>
</div>
```

Virgin Media | 2 | Freedom Pop | 24
Three | 3 | LycaMobile | 22
O2 | 5 | Plusnet | 25
Vodafone | 7 | Sky | 26
EE | 10 | giffgaff | 13
BT | 17 | Pop Telecom | 16
ID | 18 | Lebara | 28


## Tracking and Reporting

There’s no need to add your own tracking into the content units; we will attribute
your tracking ID to all outbound links for deals within the content units.

You will get automatic access to the Stickee Comparison reporting suite, allowing
you to view and analyse your clicks, orders and sales.

## Styling

All content units can be styled according to your website’s branding. There’s no
need for you to style the content unit yourself; simply tell us your colour
palette/style guide and this will be applied by Stickee.

We can supply a full list of elements which can be individually styled.

##Further Support

For further information about Stickee Comparison content units, please contact
[info@stickeecomparison.co.uk](mailto: info@stickeecomparison.co.uk).
