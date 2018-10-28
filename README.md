#### Beamer devcon iv

This repository contains the Beamer version of the devcon iv presentation
template, based on the original keynote files.

The template uses the Metropolis theme.

#### Features

The following features are present for Beamer:
- Dark/light theme
- Small logo on top left of title frame
- Template background for all slides
- Colorful logo instead of item bullets
- Standout slide
- Large logo on the right side of title frame
- Colorful bar on section break
- GitHub, Email and Twitter info on title frame
- New fonts

To do:
- Use better images for template background, title image and standout background
- Use correct GitHub/Email/Twitter icons depending on theme automatically
 
What will not be done:
- Diagrams
- Timeline
- Boxes

These can be done using standard Beamer and Tikz features.

#### Usage

##### Dark/Light theme
Change the color theme with `\metroset{background=theme}` where `theme` may be
`dark` or `light`. Default is `dark`.

##### Section page
Change the section page with `\metroset{sectionpage=page}` where `page` may be
`none` (no section page), `simple` (just section name) or `progressbar` (uses
colorful bar). Default is `progressbar`.

##### Standout slide
Apply `[standout]` to a frame. Example:
```
\begin{frame}[standout]
Really important thing!!
\end{frame}
```

Please see `template.tex` for examples and how to change whatever you might
want to change regarding images, opacity, etc.
Also, check Metropolis' documentation for full usage.

#### Compilation

To generate the presentation pdf, run
`$ make`
