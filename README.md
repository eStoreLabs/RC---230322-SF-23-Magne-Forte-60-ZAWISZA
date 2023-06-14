# 230322 SF 23 Magne Forte 100 adaptacja na aptekę zawiszy
Forte 60 będzie tak samo
## LIVE SITE LINK 
<!-- please enter link to site preview here -->
[Project live site](https://estorelabs.github.io/RC---230322-SF-23-Magne-Forte-100-GENERIC/)
## PROJECT PREVIEW
[Design preview for the project](./link)


### LINKS TO DESIGNS (in .xd or .psd)
<!-- please enter link to preview designs -->


### DESTINATION (name of e-retailer or general/pure)
Zawisza

[links to cross sell](https://docs.google.com/document/d/1mfaIbPRtbNhA-xgUddpkidL6_3wa9NOtg2awamXUlXo/edit)

[alt texts](https://docs.google.com/spreadsheets/d/13svejf7RQVbeOfPec-SE1x5KmX_7K80Q/edit#gid=213550958)

### E-RETAILER’S SPECIFICATION (technical guidelines; html, css, graphics, photos, resolution)
<!-- please enter any additional comments important for the project -->
Osobnego designu nie mam, będzie taki sam jak na Melissa tylko bez sekcji selfcare. Bez tego:
"jak radzić sobie ze stresem?" i linki do bloga (bo to tylko Melissy blog jest)

## APTEKA ZAWISZY

They use wysiwyg code editor

1. Supports only HTML4 code!

2. Do not use `<span>` tags, they are deleted. //test: try to use `<em>` tag instead with `font-style: normal`.

3. JavaScript,CSS and  images have to be from outside source ( ex. dropbox etc)

4. Avoid adding similar code next to another without <div> container


instead of:
`<a></a>`
`<a></a>`
`<a></a>`

Do this:

`<div><a></a></div>`
`<div><a></a></div>`
`<div><a></a></div>`

5. Do not use `<h1>,<h2>, <h3>` ets. tags   use `<p>` only

6. Implement style file from outside source by using below code:
```
 <script>
      function getStyles(href) {
        var head = document.getElementsByTagName("head")[0];
        var link = document.createElement("link");
        link.rel = "stylesheet";
        link.type = "text/css";
        link.href = href;
        head.appendChild(link);
      }
      document.onreadystatechange = function () {
        if (document.readyState === "complete") {
          getStyles(
            // "https://dl.dropboxusercontent.com/s/ge9zju2nmxuehnf/style.css?dl=0"
          );
        }
      };
    </script>
```
  7. Make sure to close `<img>` and `<a>` tags in one line. If not they close them in their editor by adding additional `„/>”` (default action)
  
  8. Do not use external source code: sliders/carousels from slider.js, slick-carousel, owl carousel etc. Needs to be coded without external sources.
