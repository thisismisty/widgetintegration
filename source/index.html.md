---
title: Stickee Widget
search: true
toc_footers:
  - <a href="mailto:hello@stickee.co.uk">Powered by Stickee</a>
---
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
[Mobiles demo 1](http://example.stickeemobiles.co.uk/?widget=full)

[Mobiles demo 2](http://example.stickeemobiles.co.uk/?widget=mini-5)

The content units are fully responsive, and can be inserted into any page within any
sized container.

## Installation

### JS Script

On the page or template you want the widget to appear add the following code to the &lt;head&gt; section of the page:

```html
<script src="//stickee-comparison.s3-eu-west-1.amazonaws.com/widget/stickee-comparison-widget-min.js" async></script>
```

This JS snippet only needs to be added once if you are taking both a mobiles and broadband widget.

### HTML Placeholder

The script will look for a HTML element with the class <code>.stickee-comparison-widget</code> and replace this with the widget. The HTML element contains parameters that define the behaviour of the widget. Please note, the params provided are all required.

#### Broadband

Please insert the following placeholder element in the page or template where you would like the widget to appear:

```html
<div class="stickee-comparison-widget"
    data-sector="broadband"
    data-partner="example"
    data-type="mini"
    data-width="500">
</div>
```

You can change the data-width parameter to suit the layout of your page- this can also be a percentage if required. The widget's height will change dynamically based on the content served. **It is recommended that you don’t apply a fixed width unless required.**

There are two options for 'data-type': "full" or "mini." "Mini" reveals the postcode checker initially, then once a postcode has been entered, the results are displayed below.

#### Mobiles

Please insert the following placeholder element in the page or template where you would like the widget to appear:

```html
<div class="stickee-comparison-widget"
    data-sector="mobiles"
    data-partner="example"
    data-type="mini-5"
    data-width="500">
</div>
```


You can change the data-width parameter to suit the layout of your page- this can also be a percentage if required. The widget's height will change dynamically based on the content served. It is recommended that you don’t apply a fixed width unless required.

There are two options for 'data-type': "full" or "mini." "Mini" allows you to choose how many deals your widget displays by default on page load, for example “Mini-5” will display 5 deals, whist “Mini-1” will display 1 deal.

## Pre-filtering deals

### Broadband

The following HTML snippets can be used to pre-filter broadband widgets based on package type.

#### Broadband Only

> Broadband Only

```html
<div class="stickee-comparison-widget"
   data-sector="broadband"
   data-partner="example"
   data-type="mini"
   data-width="500"
   data-filters="filters[dealtype]=broadband">
</div>
```

This will display broadband only deals by default on page load.

#### Broadband and Phone

> Broadband and Phone

```html
<div class="stickee-comparison-widget"
   data-sector="broadband"
   data-partner="example"
   data-type="mini"
   data-width="500"
   data-filters="filters[dealtype]=broadband-phone">
</div>
```

This will display broadband and phone deals by default on page load.


#### Broadband, Phone and TV

> Broadband, Phone and TV

```html
<div class="stickee-comparison-widget"
   data-sector="broadband"
   data-partner="example"
   data-type="mini"
   data-width="500"
   data-filters="filters[dealtype]=broadband-phone-tv">
</div>
```

This will display broadband, phone and TV deals by default on page load.

#### Business broadband deals

> Business broadband

```html
<div class="stickee-comparison-widget"
   data-sector="broadband"
   data-partner="example"
   data-feed="business"
   data-type="mini"
   data-width="500"
   data-filters="">
</div>
```

This will display broadband for businesses only.

#### Providers

> Providers

```html
<!-- For providers, use the following code: -->
<div class="stickee-comparison-widget"
   data-sector="broadband"
   data-partner="example"
   data-type="mini"
   data-width="500"
   data-filters="filters[suppliers][]=supplierID">
</div>
```

The following HTML snippets can be used to pre-filter broadband widgets.

| Supplier     | Supplier ID | Supplier             | Supplier ID |
|--------------|-------------|----------------------|-------------|
| BT           | ba3lLMM2yA  | First Utility        | eyxlnJmlNP  |
| Virgin Media | OBxpm3Zl97  | John Lewis Broadband | WPXpDwR2DN  |
| Plusnet      | Zy1j09olB8  | Now TV               | zGe2GRylMb  |
| Sky          | eDnjZ9VpAr  | Origin Broadband     | WyPloLA2zL  |
| TalkTalk     | LwKpE0x25E  | Post Office          | VE6jk6bpBr  |
| EE           | eDnjZVVjAr  | SSE                  | 8ryp8nxl0x  |
| Direct Save  | QvV2OQPjGD  | Vodafone             | KNvj4MPlX4  |

<aside class="notice">
Please remember to replace &lt;data-partner&gt; with your partner ID.
</aside>

### Mobiles

The following HTML snippets can be used to pre-filter mobiles widgets based on makes and models and networks.

#### SIM Only widget

> SIM Only widget

```html
<!-- The following HTML snippet can be used to create a widget which defaults to SIM Only and shows 4 deals -->
<div class="stickee-comparison-widget"
            data-sector="mobiles"
            data-partner="example"
            data-type="mini-4"
            data-dealtype="simo">
</div>
```

You can create a widget which defaults to SIM Only deals on page load.

#### Makes

> Makes

```html
<!-- The following HTML snippet can be used to pre-filter mobiles widgets based on make -->
<div class="stickee-comparison-widget"
   data-sector="mobiles"
   data-partner="example"
   data-type="mini"
   data-width="500"
   data-filters="filters[make]=makeID">
</div>
```

You can create a widget which pre-filters mobiles widgets based on make.

| Make        | Make ID | Make     | Make ID |
|-------------|---------|----------|---------|
| Alcatel     | 22      | Kodak    | 62      |
| Amazon      | 61      | LG       | 6       |
| Apple       | 19      | Lenovo   | 40      |
| BlackBerry  | 2       | Motorola | 1       |
| Caterpillar | 56      | Nokia    | 4       |
| Dewalt      | 68      | Samsung  | 5       |
| Doro        | 42      | Sony     | 54      |
| Google      | 15      | Vodafone | 26      |
| HP          | 35      | WileyFox | 66      |
| HTC         | 13      | ZTE      | 8       |
| Huawei      | 12      |          |         |

#### Models

> Models

```html
<!-- The following HTML snippet can be used to pre-filter mobiles widgets based on make and model -->
<div class="stickee-comparison-widget"
   data-sector="mobiles"
   data-partner="example"
   data-type="mini"
   data-width="500"
   data-filters="filters[make]=makeID&filters[model]=modelID">
</div>
```

You can create a widget which pre-filters mobiles widgets based on model.

A full list of available models can be downloaded [here](https://docs.google.com/a/stickee.co.uk/spreadsheets/d/1940lJPcX8wB7BAhmeHTN4UzF-vlioNaa6sOJgpjLojA/edit?usp=sharing).


#### Networks

> Networks

```html
<!-- The following HTML snippet can be used to pre-filter mobiles widgets based on networks. -->
<div class="stickee-comparison-widget"
   data-sector="mobiles"
   data-partner="example"
   data-type="mini"
   data-width="500"
   data-filters="filters[networks]=networkID">
</div>
```

You can create a widget which pre-filters mobiles widgets based on network.

| Network      | Network ID | Network     | Network ID |
|--------------|------------|-------------|------------|
| Virgin Media | 2          | Freedom Pop | 24         |
| Three        | 3          | LycaMobile  | 22         |
| O2           | 5          | Plusnet     | 25         |
| Vodafone     | 7          | Sky         | 26         |
| EE           | 10         | giffgaff    | 13         |
| BT           | 17         | Pop Telecom | 16         |
| ID           | 18         | Lebara      | 28         |

<aside class="notice">
Please remember to replace &lt;data-partner&gt; with your partner ID.
</aside>


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

# Stickee Speed Test Widget

## Integration
```html
<iframe src="https://widget-speedtest.stickee.co.uk/[partnername]" width="500" height="820"></iframe>
```

The Broadband Speed Test widget has been built with the intention of being integrated into partner websites by way of an iFrame.
The following iFrame example should have `[partnername]` replaced with a valid partner. If omitted, the widget will load a default ‘stickee’ branded Speed Test.

Please note that this product is in beta and should be placed within a container with a width of 350px max in order to display across all breakpoints.

## Configuration
The speed test has configurable elements to change the look and feel to match a partner’s website. The following elements can be configured:

|Variable|Description|Example|
|--------|-----------|-------|
|Gauge Colours|The colours used in the speed gauge. <br> <br>These are split into 3 separate; slow, average and fast (to denote the speed category of the broadband. <br><br> The colours are used as follows: <br> `slow` is used in the 0 to 20Mbs segment of the gauge. <br>`average` and `fast` are used to generate a gradient between 20Mbs and 140Mbs with fast being used as a solid colour thereafter|`slow: '#bf5345'` <br>`average: '#82a8bd'` <br>`fast: '#2f6e91'`|
|Body font|The font URL and font-family declaration used for the general text within the speed test|This must be a Google font.|
|CTA Colours|The colours used in the CTA (Start Test button). These are split into `background` and `text`|`background: '#5aaf0b'` <br>`text: '#ffffff'`|

![Speedtest Gauge](https://s3-eu-west-1.amazonaws.com/stickee-comparison/docs/speed-test/speedtest.png "Speedtest Gauge")

# Further Support

For further information about Stickee Comparison content units, please contact
<a href="mailto:hello@stickee.co.uk">hello@stickee.co.uk</a>.
