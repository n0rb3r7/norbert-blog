+++
authors = ["Norbert Stange"]
date = 2020-08-06T03:00:00Z
excerpt = "My first expreience working with these three tools"
draft = "true"
hero = "/images/1500x500.jpg"
timeToRead = 3
title = "My first encounter with Hugo, Netlify and Forestry"

+++
# The triplet

For all those who know a little something and have started creating sites with Hugo, Netlify and Forestry, here comes my experience and the bumps I came across in my road.

Hugo Static Site Generator v0.74.3-DA0437B4 windows/amd64 BuildDate: 2020-07-23T16:23:30Z


This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.
<!--more-->
{{< highlight html >}}
<script>
var date = new Date();
var year = date.getFullYear();
var month = date.getMonth();
var day = date.getDate();
var minDate;

$('#from_date').datepicker({
  format: 'dd mmm yyyy',
  minDate: date,
  setDefaultDate: date,

  onSelect: function () {

    var toYear = this.date.getFullYear();
    var toMonth = this.date.getMonth();
    var toDay = this.date.getDate();
    minDate = new Date(toYear, toMonth, toDay);

    $("#to_date").datepicker({
      format: 'dd mmm yyyy',
      setDefaultDate: minDate,
      minDate: minDate,
    })
  }
});
</script>
{{< /highlight >}} 

## Headings

The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

# H1
## H2
### H3
#### H4
##### H5
###### H6


<img class="Image__Small" src="/images/1500x500.jpg"/>

## Paragraph

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.


## Code Blocks

#### Code block with backticks

```html
html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

#### Code block with Hugo's internal highlight shortcode
{{< highlight html >}}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p id="one">Test</p>
  <script>
    element = document.getElementById(one);
  </script>
</body>
</html>
{{< /highlight >}}

