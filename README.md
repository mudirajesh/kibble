# Netflix Clone

Replica of the Netflix website created as a light HTML CSS and JS exercise - [Check it out](https://kibble.netlify.app/)

[![Practice](https://img.shields.io/badge/Practice-HTML/CSS/JS-orange.svg)](https://kibble.netlify.app/)

_<p align="center">"Enjoying a website for entertainment... yum yum yum"</p>_

<div align="center" style="text-align:center; margin:auto;">
<img align="center" src="https://bit.ly/43CH0eS" width="150"/>

</div>
<img align="center" src="./img/logo.png" width="150"/>

## Summary

A simple warm-up exercise to practice building a clone of the Netflix Homepage using the following technologies:

- HTML
- CSS
- Vanilla JS - ES6
- Simply for the love of coding :-)

## Functionality

- It aims to look aesthetically pleasing, and that's about it :-)

## Key Learning Points

- CSS Grid
- Styling Tables
- Tab functionality with Javascript
- Positioning

## Notable Features

Typically, developers often resort to CSS Frameworks to create and style tabs and switch between them. However, here's a straightforward and fundamental approach to implement switchable tab content using Vanilla JS:

```javascript
const tabItems = document.querySelectorAll(".tab-item");
const tabContentItems = document.querySelectorAll(".tab-content-item");

// Select tab content
function selectItem(e) {
  removeBorder();
  removeShow();

  // Add border to the current tab
  this.classList.add("tab-border");

  // Retrieve corresponding content item from the DOM
  const tabContentItem = document.querySelector(`#${this.id}-content`);

  // Apply show class
  tabContentItem.classList.add("show");
}

function removeBorder() {
  tabItems.forEach(item => item.classList.remove("tab-border"));
}

function removeShow() {
  tabContentItems.forEach(item => item.classList.remove("show"));
}

// Listen for tab click
tabItems.forEach(item => item.addEventListener("click", selectItem));
```

As for the HTML, you only need the following:

```html

<!-- The content is quite lengthy, so I will add it later -->
<!-- But here's the basic idea -->

<div class="tab-item">

  <!-- Selectors for different tab content -->
</div>
<div class="tab-content-item">

  <!-- Content for each tab item -->
</div>

<!-- Simply add more selectors and corresponding 
tab content for each selector -->
```

> Additionally (Just a thought), you could enhance this further by adding animations to the selector borders, etc.

## Upcoming Features

If I ever revisit this project, I might add the remaining pages of the Netflix website.

## Contribution

Contributions are highly welcomed. Feel free to fork, clone, make pull requests, report issues, etc.

## Acknowledgments

- Special thanks to [@anjelayu] for his incredible courses 
  

That being said
_<p align="center">To the Front... to the Back... End to End... no slacking. Making ends meet. lol</p>_
