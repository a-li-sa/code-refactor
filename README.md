# 01 HTML CSS Git: Code Refactor

For this marketing agency, I refactored an existing webpage to follow accessibility standards, optimizing the site for search engines.

In this webpage, I ensured that links function correctly, CSS follows the semantic structure of HTML, CSS selectors and properties are consolidated, and comments are included before each element or section of the page.

GIVEN a webpage meets accessibility standards
- [x] WHEN I view the source code THEN I find semantic HTML elements
- [x] WHEN I view the structure of the HTML elements THEN I find that the elements follow a logical structure independent of styling and positioning
- [x] WHEN I view the image elements THEN I find accessible alt attributes
- [x] WHEN I view the heading attributes THEN they fall in sequential order
- [x] WHEN I view the title element THEN I find a concise, descriptive title

## Summary

* [Installation](#installation)
* [Usage](#usage)
* [Changes in HTML](#changes-in-index.html)
* [Changes in CSS](#changes-in-style.css)
* [Credits](#credits)

## Installation

To look at the webpage, you can click [here](https://a-li-sa.github.io/code-refactor/).

## Usage 

Scroll or click on the navigation links in the webpage to view the content. 

## Changes in index.html 

### new html / old html

line 8 / line 7
- changed title from `"website"` to `"Horiseon Social Solution Services. Inc."`

line 14 / line 11
- semantic HTML: changed `<div class="header">` to `<header>`

line 19 / line 13
- semantic HTML: changed `<div>` to `<nav>`

line 34 / line 25
- semantic HTML: changed `</div>` to `</nav>`

line 36 / line 26
- semantic HTML: changed `</div>` to `</header>`

line 42 / line 28
- semantic HTML: changed `<div class="content">` to `<main>`

line 45 / line 29
- semantic HTML: changed div tag to section tag
- changed class from `"search-engine-optimization"` to `"content"`
- added `id="search-engine-optimization"` inside section tag so that the tag could be linked to href from line 24 / line 16

line 46 / line 30
- added alt attribute inside img tag 
- `alt="Backlink, content, headings, mobile compatibility, social media, and link building are all related to SEO."`

line 51 / line 35
- semantic HTML: changed `</div>` to `</section>`

line 54 / line 36
- semantic HTML: changed div tag to section tag
- changed class from `"online-reputation-management"` to `"content"`

line 55 / line 37
- added alt attribute inside img tag 
- `alt="Reputation can be visualized on bar and pie graphs."`

line 60 / line 42
- semantic HTML: changed `</div>` to `</section>`

line 63 / line 43
- semantic HTML: changed div tag to section tag
- changed class from `"social-media-marketing"` to `"content"`

line 64 / line 44
- added alt attribute inside img tag 
- `alt="Many icons and words are associated with social media."`

line 69 / line 49
- semantic HTML: changed `</div>` to `</section>`

line 71 / line 50
- semantic HTML: changed `</div>` to `</main>`

line 74 / line 51
- semantic HTML: changed `<div class="benefits">` to `<aside>`
- removed class attribute

line 77 / line 52
- semantic HTML: changed div tag to section tag
- changed class from `"benefit-lead"` to `"benefits"`

line 78 / line 53
- changed `<h3>` , `</h3>` to `<h2>` , `</h2>`

line 79 / line 54
- added alt attribute inside img tag
- `alt="Lead Generation is represented by an icon of a sales funnel."`

line 83 / line 58
- semantic HTML: changed `</div>` to `</section>`

line 86 / line 59
- semantic HTML: changed div tag to section tag
- changed class from `"benefit-brand"` to `"benefits"`

line 87 / line 60
- changed `<h3>` , `</h3>` to `<h2>` , `</h2>`

line 88 / line 61
- added alt attribute inside img tag
- `alt="Brand Awareness is represented by an icon that shows a glowing lightbulb as the head of a body."`

line 92 / line 65
- semantic HTML: changed `</div>` to `</section>`

line 95 / line 66
- semantic HTML: changed div tag to section tag
- changed class from `"benefit-cost"` to `"benefits"`

line 96 / line 67
- changed `<h3>` , `</h3>` to `<h2>` , `</h2>`

line 97 / line 68 
- added alt attribute inside img tag
- `alt="Cost Management is represented by an icon that shows a gear and dollar coins."`

line 101 / line 72
- semantic HTML: changed `</div>` to `</section>`

line 103 / line 73
- semantic HTML: changed `</div>` to `</aside>`

line 106 / line 74
- semantic HTML: changed `<div>` to `<footer>`

line 111 / line 79
- semantic HTML: changed `</div>` to `</footer>`

---

added comments on lines 4, 11, 18, 21, 38, 41, 44, 53, 62, 73, 76, 85, 94, 105

## Changes in style.css 

### new css / old css

line 13 / line 49
  - moved `p` selector, after the `body` selector

lines 19, 26, 31 / lines 11, 18, 23
  - renamed `.header` to `header`

lines 37, 45, 49 / lines 27, 35, 39
  - renamed `.header div` to `nav`

line 82 / line 72
  - renamed `.content` to `main`
  - moved `main` selector, after the `.float-right` selector

line 90 / lines 164, 168, 172
  - the following selectors shared the same properties: `.search-engine-optimization img` , `.online-reputation-management img` , `.social-media-marketing img`
  - moved the above mentioned selectors, after the `main` selector
  - consolidated the three selectors to a single `.content img` selector, which contains the same properties

line 94 / lines 176, 181, 186
  - the following selectors shared the same properties: `.search-engine-optimization h2` , `.online-reputation-management h2` , `.social-media-marketing h2`
  - moved the above mentioned selectors, after the `.content img` selector
  - consolidated the three selectors to a single `.content h2` selector, which contains the same properties

line 99 / lines 137, 146, 155
  - the following selectors shared the same properties: `,search-engine-optimization` , `.online-reputation-management` , `.social-media-marketing`
  - moved the above mentioned selectors, after the `.content h2` selector
  - consolidated the three selectors to a single `.content` selector, which contains the same properties 

line 110 / line 78
  - renamed `.benefits` to `aside`

line 123 / lines 104, 109, 114
  - the following selectors shared the same properties: `.benefit-lead h3` , `.benefit-brand h3` , `.benefit-cost h3`
  - moved the above mentioned selectors, after the `aside` selector
  - consolidated the three selectors to a single `.benefits h2` selector, which contains the same properties

line 126 /
  - added new property `font-size` with value `18.72px`

line 129 / lines 119, 125, 131
  - the following selectors shared the same properties: `.benefit-lead img` , `.benefit-brand img` , `.benefit-cost img`
  - moved the above mentioned selectors, after the `.benefits h2` selector
  - consolidated the three selectors to a single `.benefits img` selector, which contains the same properties

line 135 / lines 89, 94, 99
  - the following selectors shared the same properties: `.benefit-lead` , `.benefit-brand` , `.benefit-cost`
  - moved the above mentioned selectors, after the `.benefits img` selector
  - consolidated the three selectors to a single `.benefits` selector, which contains the same properties

lines 142, 149 / lines 191, 198
  - changed `.footer` to `footer`

---

added comments on lines 7, 17, 35, 59, 88, 108, 121, 140

## Credits

The HTML and assets were provided by 2019 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.

## License 

MIT License Copyright (c) 2020 Alisa Poon
