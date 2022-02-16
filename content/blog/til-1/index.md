---
title: Today I Learned - html <details>
date: "2022-02-15T20:12:03.284Z"
description: "TIL about html details tag"
---

In "Today I learned" series I would like to share some small stuff I just learned when going through my internet feeds.

The ```details``` tag enables easy way to have some expandable content without any js, it's pure html.

Let's take a look at following code snippet:

```html
<details>
    <summary>Summary - click to expand</summary>
    <p>Basically any html content can be put here, i.e. list</p>
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
    </ul>
</details>
```

That gives us following:

<div class="details">
    <details>
        <summary>Summary - click to expand</summary>
        <p>Basically any html content can be put here.</p>
        i.e. list
        <ul>
            <li>Item 1</li>
            <li>Item 2</li>
        </ul>
    </details>
</div>

<br/>

It can be open by default with just adding the ```open``` attribute

```html
<details open>
    <summary>Summary - already open</summary>
    <p>The inner content.</p>
</details>
```

<br/>
<p>and the result is:</p>

<div class="details">
    <details open>
        <summary>Summary - already open</summary>
        <p>The inner content.</p>
    </details>
</div>

<br/>
<p>Of course it doesn't look exactly pretty without any additional styling so let's tweak it a little.</p>

<div class="details tweaked">
    <details>
        <summary>Summary - click to expand</summary>
        <h4>Reasons to use this:</h4>
        <ul>
            <li>It's simple</li>
            <li>It's easy</li>
            <li>It's fun</li>
        </ul>
    </details>
</div>