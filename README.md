# Materialize-Css Summary

Materialize CSS From Scratch With 5 Projects by Brad Traversy

I am going to write down the parts I want to write 😐

# Details

<details open>
  <summary>Click to Contract/Expend</summary>

### 3. Environment Setup

- Install Live Server Extension
- Emmet!!

[Emmet Cheat Sheet](https://docs.emmet.io/cheat-sheet/)

### 4. Materialize Sandbox Setup

This course is using v0.100.2 and v1.0.0 the latest one.

[Upgrade from 0.100.2](https://github.com/Dogfalo/materialize/blob/v1-dev/v1-upgrade-guide.md)

### 5. Typography & Alignment

[Flow Text](https://materializecss.com/typography.html) \
-> text-size : Fully responsive text size

[Vertical Align](https://materializecss.com/helpers.html) \
-> valign-wrapper : assign wrapper

[Clearfix](https://getbootstrap.com/docs/5.0/helpers/clearfix/) \
-> Is it from bootstrap?

### 7. Buttons & Icons

Two ways to use icons : Slightly different

1. material-icons
2. font-awesome

```html
<!--Import Google Icon Font-->
<link
  href="https://fonts.googleapis.com/icon?family=Material+Icons"
  rel="stylesheet"
/>
<link
  href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css"
  rel="stylesheet"
  integrity="sha384-wvfXpqpZZVQGK6TAh5PVlGOfQNHSoD2xbE+QkPxCAFlNEevoEH3Sl0sibVcOQVnN"
  crossorigin="anonymous"
/>

<!-- BUTTON WITH MATERIAL ICON -->
<a class="btn waves-effect waves-light" href="#!">
  <i class="material-icons right">shopping_cart</i> Buy Now</a
>
<!-- BUTTON WITH FONT AWESOME ICON -->
<a class="btn waves-effect waves-light" href="#!">
  <i class="fa fa-shopping-cart left"></i> Buy Now</a
>
```

### 8. Floating & Fixed Action Buttons

This is an awesome feature.

[Floating Action Button](https://materializecss.com/floating-action-button.html)

```js
$(document).ready(function () {
  $('.fixed-action-btn').openFAB(); // FAB : Floating Action Button
  $('.fixed-action-btn').closeFAB();
  $('.fixed-action-btn').openToolbar();
  $('.fixed-action-btn').closeToolbar();
});
```

### 9. Navbar

Tip: if container div is used inside nav-wrapper

```html
<div class="nav-wrapper">
  <div class="container">
    <a>Logo</a>
    <ul>
      <li>Logo</li>
    </ul>
  </div>
</div>
```

### 11. The Grid System

#### Screen Sizes

|                   |  Mobile  | Tablet  | Desktop | Large Desktop |
| :---------------- | :------: | :-----: | :-----: | :-----------: |
| Range             | <= 600px | > 600px | > 992px |   > 1200px    |
| Class Prefix      |    .s    |   .m    |   .l    |      .xl      |
| Container Width   |   90%    |   85%   |   70%   |      70%      |
| Number of Columns |    12    |   12    |   12    |      12       |

### 14. Basic Form & Input Controls

```js
// Email validation
<input placeholder="Email" id="email" type="email" class="validate" />
<label data-error="Invalid" data-success="Valid" for="email">Email</label>

// To use select options
$('select').material_select();

// widh-gap, Radio button
<input type="radio" name="gender" id="male" checked />
<input class="with-gap" type="radio" name="gender" id="female" />

// filled-in, Checkbox
<input type="checkbox" name="tech" id="css" checked />
<input type="checkbox" class="filled-in" name="tech" id="js" />
```

### 15. Fancy Form & Input Controls

#### Many useful features

```js
// INIT DATEPICKER
$('.datepicker').pickadate({});

// INIT TIMEPICKER
$('.timepicker').pickatime({});

// INIT AUTOCOMPLETE
$('.autocomplete').autocomplete({});
```

### 19. Carousel

[Carousel](https://materializecss.com/carousel.html)

### 20. Collapsible

[Collapsible](https://materializecss.com/collapsible.html)

There's one more type : popout on v1.0.0

### 24. Modals

[Modals](https://materializecss.com/modals.html)

### 30. Project Intro

- p1_travelville_v0.100.2
  1. Materializecss v0.100.2
  2. jQuery
  3. Font Awesome v5.0.6
- p1_travelville_v1.0.0
  1. Upgrading to v1.0.0
  2. Using vanila javascript
  3. Font Awesome Free v5.15.3

### 32. Image Slider

[Pexels](https://www.pexels.com/) : Free images and videos
[Unsplash](https://unsplash.com/) : Free images and videos

[Materialize CSS Slider - Media](http://archives.materializecss.com/0.100.2/media.html)

### 33. Search & Icon Boxes

[Materialize CSS Autocomplete](https://materializecss.com/autocomplete.html)

!important : to overwrite material css default style

### 34. Popular Places & Gallery

fa-4x : font awesome size x 4

[Unsplash Fetching Random Image](https://source.unsplash.com/1600x900/?beach)

### 37. Navbar & Showcase

- v0.100.2
  - Default Font Family: Roboto
- v1.0.0
  - Default font awesome size is bigger compare to v0.100.2
  - Default Font Family: -apple-system

```html
<!-- v1.0.0 -->
<!-- Smaller Size -->
<li><a href="https://facebook.com" class="fab fa-facebook"></a></li>
<!-- Bigger Size -->
<li>
  <a href="https://facebook.com">
    <i class="fab fa-facebook"></i>
  </a>
</li>
```

### 44. Navbar & Sidenav

[What is The Fastest Way to Load Javascript : Defer](https://youtu.be/BMuFBYw91UQ)

![Script Defer](./resources/script-load.png)

### 46. Display Chart & Recent Comments

[Canvas JS - Simple Line Chart](https://canvasjs.com/html5-javascript-line-chart/)

### 58. Koala Setup & Sass

Installing Live Sass Compiler (VS Extension) \
(I did not install Koala)

Its own settings are saved on .vscode/settings.json

[vscode-live-sass-compiler Settings](https://github.com/ritwickdey/vscode-live-sass-compiler/blob/master/docs/settings.md)

</details>

## What I have used

- Unsplash : Fetching Random Image
- Canvas JS : Line Chart and Pie Chart

## Next Step

- Upload separate posts on getsby website.
  - Git commands
  - Terminal commands
  - Material css tips
- Patron Project
  - Add chips (3_6_chips_pagination.html)
