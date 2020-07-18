+++
# A Projects section created with the Portfolio widget.
widget = "portfolio"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 65  # Order that this section will appear.

title = "Projects"
subtitle = ""

[content]
  # Page type to display. E.g. project.
  page_type = "project"

  # Filter toolbar (optional).
  # Add or remove as many filters (`[[content.filter_button]]` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `[[content.filter_button]]` below.

  # Default filter index (e.g. 0 corresponds to the first `[[filter_button]]` instance below).
  filter_default = 0

  # [[content.filter_button]]
  #   name = "All"
  #   tag = "*"

  # [[content.filter_button]]
  #   name = "Deep Learning"
  #   tag = "Deep Learning"

  # [[content.filter_button]]
  #   name = "Other"
  #   tag = "Demo"

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "2"

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   5 = Showcase
  view = 3

  # For Showcase view, flip alternate rows?
  flip_alt_rows = false

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.

  # Background color.
  # color = "navy"

  # Background gradient.
  # gradient_start = "DeepSkyBlue"
  # gradient_end = "SkyBlue"

  # Background image.
  # image = "background.jpg"  # Name of image in `static/img/`.
  # image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.

  # Text color (true=light or false=dark).
  # text_color_light = true  

[advanced]
 # Custom CSS. 
 css_style = ""

 # CSS class.
 css_class = ""
+++

1. PDL**
   - This project proposes an efficient PBD-based (Pairwise Block Design) Data Layout, PDL, to speed up data repair for single node failure in mixed erasure-coded distributed storage systems. It achieves almost uniform distribution, and higher repair performance due to reduced cross-rack traffic and load balance of read and write I/Os during repair process.
   - I design the data distribution method, and the corresponding failure recovery scheme. And I also implement them in Hadoop 3.1.1. 

2. **SelectiveEC**
   - This project proposes a balanced scheduling module, SelectiveEC, to dynamically select some stripes to be reconstructed in a batch, and select source and replacement nodes for each reconstruction task. It achieves balanced network recovery traffic, computing resources and disk I/Os against single node failure in erasure-coded storage systems.
   - I design the scheduling algorithm, build the SelectiveEC prototype and validate it by simulation. 

3. **D<sup>3</sup>**
   - The proposed distribution D<sup>3</sup> uniformly distributes data/parity blocks among nodes in large scale erasure-coded distributed storage systems, and minimizes the cross-rack repair traffic against a single node failure. 
   - I integrate the distribution D<sup>3</sup> into HDFS-EC module of Hadoop 3.1.0 and evaluate the repair performance over Reed-Solomon codes. In the journal version, I extend it to locally repairable codes, provide efficient strategy to maintain the D<sup>3</sup> data layout after recovery, and conduct more experimental evaluations.

4. **A note on one weight and two weight projective Z<sub>4</sub>-codes.**
   - This is the work in my undergraduate.
   - I solve the open problems about algebraic codes, moreover, I work out the diophantine problem and then give the sufficient conditions for the nonexistence of two-Lee weight projective codes over Z<sub>4</sub> with type 4<sup>k<sub>1</sub></sup>2<sup>k<sub>2</sub></sup>. 