![alt text](https://afterburner.io/stoker-git.svg "Stoker - A svg iconset")
#### Stoker
A svg iconset

## Getting started
Class based structure in order to change/add styles to icon.
```
+-- svg
|   +-- .stroke (group)
|       +-- outline (stroke)
|   +-- .bg (group)
|       +-- .near (fill)
|       +-- .middle (fill)
|       +-- .far (fill)
```

#### Example

![Styling example](https://raw.githubusercontent.com/psilore/stoker/master/src/example/example-class-styling.svg)


SVG
```
<svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 28 28">
  <g fill="none" fill-rule="evenodd" class="example">
    <g class="image">
      <g fill="#FF00C8" class="bg">
        <rect width="28" height="28" class="far" opacity=".152" rx="2"/>
        <circle cx="7.5" cy="6.5" r="2.5" fill-opacity=".5" class="middle"/>
        <polygon fill-opacity=".9" points=".875 22.75 8.75 14.438 12.688 18.813 19.25 11.813 27.125 20.125 27.125 27.125 .875 27.125" class="near"/>
      </g>
      <g stroke="#810076" stroke-width="2" class="stroke">
        <circle cx="7.5" cy="6.5" r="2.5" class="sun-stroke"/>
        <polyline points="1 23 9 15 13 19 19 12 27 21" class="mountain-stroke"/>
        <rect width="26" height="26" x="1" y="1" class="square-stroke" rx="2"/>
      </g>
    </g>
  </g>
</svg>
```

CSS
```
:root {
    --primary-color: rgb(129, 0, 118);
    --dark-color: rgba(255, 0, 200, .9);
    --normal-color: rgba(255, 0, 200, .5);
    --light-color: rgba(255, 0, 200, .15);
}

svg g[class*="stroke"],
svg rect[class*="stroke"],
svg path[class*="stroke"] {
    stroke: var(--primary-color);
    stroke-linejoin: miter;
    stroke-width: 2;
}

svg g[class*="far"],
svg rect[class*="far"],
svg path[class*="far"],
svg polyline[class*="far"],
svg circle[class*="far"] {
    fill: var(--light-color);
}

svg g[class*="middle"],
svg rect[class*="middle"],
svg path[class*="middle"],
svg polyline[class*="middle"],
svg circle[class*="middle"] {
    fill: var(--normal-color);
}

svg g[class*="near"],
svg rect[class*="near"],
svg path[class*="near"],
svg polyline[class*="near"],
svg circle[class*="near"],
svg polygon[class*="near"] {
    fill: var(--dark-color);
}
```


## Icons

#### Heart
![Heart icon](https://raw.githubusercontent.com/psilore/stoker/master/src/svg/heart.svg)
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 32 32">
  <g fill="none" fill-rule="evenodd" class="stoker">
    <g fill-rule="nonzero" class="icon" transform="translate(-16 -176)">
      <g class="heart" transform="translate(18 180)">
        <path fill="#D8D8D8" d="M20.851.764c3.611 0 6.493 3.43 6.493 7.57 0 4.14-2.201 7.886-5.451 11.106-3.25 3.22-7.429 5.06-7.893 5.06-.464 0-4.643-1.84-7.893-5.06C2.857 16.22.61 12.474.61 8.334S3.476.764 7.293.764c2.545 0 4.78 1.262 6.707 3.784C16.023 2.026 18.306.764 20.851.764z" class="near"/>
        <path stroke="#000" stroke-width="2" d="M20.611 1c-2.407 0-4.336 1.035-5.797 3.081-.327.458-.598.92-.814 1.39a8.533 8.533 0 0 0-.814-1.39C11.725 2.035 9.796 1 7.39 1c-1.774 0-3.365.76-4.513 2.003C1.708 4.268 1 6.027 1 8c0 4.235 1.922 7.508 5.207 10.793C9.416 22.002 13.536 24 14 24c.464 0 4.584-1.998 7.793-5.207C25.078 15.508 27 12.235 27 8c0-1.944-.74-3.678-1.903-4.937C23.922 1.791 22.314 1 20.61 1z"/>
      </g>
    </g>
  </g>
</svg>
```

#### Star
![Star icon](https://raw.githubusercontent.com/psilore/stoker/master/src/svg/star.svg)
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 32 32">
  <g fill="none" fill-rule="evenodd" class="stoker">
    <g class="icon" transform="translate(-80 -176)">
      <g class="star" transform="translate(82 177)">
        <polygon fill="#D8D8D8" points="14 23.225 5.966 27.667 7.5 18.26 1 11.598 9.983 10.225 14 1.667 18.017 10.225 27 11.598 20.5 18.26 22.034 27.667" class="near"/>
        <path stroke="#000" stroke-width="2" d="M14 3.02l-3.648 7.772-8.277 1.264L8.068 18.2l-1.402 8.596L14 22.741l7.334 4.054-1.402-8.596 5.993-6.143-8.277-1.264L14 3.02z"/>
      </g>
    </g>
  </g>
</svg>
```

#### Image
![Image icon](https://raw.githubusercontent.com/psilore/stoker/master/src/svg/image.svg)
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 32 32">
  <g fill="none" fill-rule="evenodd" class="stoker">
    <g class="icon" transform="translate(-16 -272)">
      <g class="image" transform="translate(18 274)">
        <g fill="#D8D8D8" class="bg">
          <rect width="28" height="28" class="far" rx="2"/>
          <circle cx="7.5" cy="6.5" r="2.5" class="middle"/>
          <polygon points=".875 22.75 8.75 14.438 12.688 18.813 19.25 11.813 27.125 20.125 27.125 27.125 .875 27.125" class="near"/>
        </g>
        <g stroke="#000" stroke-width="2" class="stroke">
          <circle cx="7.5" cy="6.5" r="2.5" class="sun-stroke"/>
          <polyline points="1 23 9 15 13 19 19 12 27 21" class="mountain-stroke"/>
          <rect width="26" height="26" x="1" y="1" class="square-stroke" rx="2"/>
        </g>
      </g>
    </g>
  </g>
</svg>
```
#### Download
![Download icon](https://raw.githubusercontent.com/psilore/stoker/master/src/svg/download.svg)
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 32 32">
  <g fill="none" fill-rule="evenodd" class="stoker">
    <g class="icon" transform="translate(-80 -272)">
      <g class="download" transform="translate(86 279)">
        <g fill="#D8D8D8" class="bg" transform="translate(5)">
          <path d="M7 1v6h3l-5 7-5-7h3V1a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1z" class="far"/>
        </g>
        <path stroke="#000" stroke-linecap="round" stroke-width="2" d="M20 14v2.5c0 .828-.497 1.5-1.111 1.5H1.11C.497 18 0 17.328 0 16.5V14" class="down-stroke"/>
        <path stroke="#000" stroke-width="2" d="M12 1v6h3l-5 7-5-7h3V1a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1z" class="arrow-stroke"/>
      </g>
    </g>
  </g>
</svg>
```
#### Magnifying glass
![Magnifying glass icon](https://raw.githubusercontent.com/psilore/stoker/master/src/svg/magnifying-glass.svg)
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 32 32">
  <g fill="none" fill-rule="evenodd" class="stoker">
    <g class="icon" transform="translate(-272 -272)">
      <g class="magnifying-glass" transform="translate(277 277)">
        <g fill="#D8D8D8" class="bg">
          <circle cx="7" cy="7" r="7" class="near"/>
        </g>
        <circle cx="7" cy="7" r="7" stroke="#000" stroke-width="2" class="lens-stroke"/>
        <line x1="12.5" x2="14.5" y1="12.5" y2="14.5" stroke="#000" stroke-linecap="square" class="rod-stroke"/>
        <line x1="15.5" x2="21.5" y1="15.5" y2="21.5" stroke="#000" stroke-linecap="round" stroke-width="3" class="handle-stroke"/>
      </g>
    </g>
  </g>
</svg>
```
