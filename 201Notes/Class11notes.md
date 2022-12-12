Video and Audio Content

According to mdn, the first video and audio contents were made possible through "proprietary plug in based technologies like Flash and Silverlight". Because of the lack of security and accessibility, those technologies are no longer used and have been replaced by HTML solutions. < video > and < audio > are two of the elements now used along with JS API's for controlling them.

Src contains a path to the video, just like using img. Using the controls attribute either lets you use the browsers built in control interface or build your own using the proper JSAPI's.

Fallbacks -

  The paragraph inside the <video> tags
  This is called fallback content — this will be displayed if the browser accessing the page doesn't support the <video> element, allowing us to provide a fallback for older browsers. This can be anything you like; in this case, we've provided a direct link to the video file, so the user can at least access it some way regardless of what browser they are using.

A Guide to Grid

  Differences between flexbox and grid layout...

   Flexbox and Grid layout can work well together 
   Grid layout is two-dimensional and flexbox is more one-dimensional 
   Flexbox can optionally wrap more efficiently
   Grid layout happens on the parent elements whereas Flex happens on the children elements
   Grid is better at overlapping and is considered sturdier 
   Flexbox can push things away

Grid Container
The element on which display: grid is applied. It’s the direct parent of all the grid items. In this example container is the grid container.

<div class="container">
  <div class="item item-1"> </div>
  <div class="item item-2"> </div>
  <div class="item item-3"> </div>
</div>

Grid Item
The children (i.e. direct descendants) of the grid container. Here the item elements are grid items, but sub-item isn’t.

<div class="container">
  <div class="item"> </div>
  <div class="item">
    <p class="sub-item"> </p>
  </div>
  <div class="item"> </div>
</div>

Grid Line
The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column.

Response Images

  By making images responsive, you allow the quality of the images (in their entirety) to be maintained regardless the size of the window. So if the window shrinks, it allows the images to respond and adjust accordingly rather than being cropped and the content being affected.

  "Srcset defines the set of images we will allow the browser to choose between, and what size each image is. Each set of image information is separated from the previous one by a comma.

    -An image filename (elva-fairy-480w.jpg)
    -A space
    -The image's intrinsic width in pixels (480w) — note that this uses the w unit, not px as you might expect. An image's intrinsic size is its real size, which can be found by inspecting the image file on your computer (for example, on a Mac you can select the image in Finder and press Cmd + I to bring up the info screen)."

  "Sizes defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true — these are the hints we talked about earlier. In this case, before each comma we write:

    -A media condition ((max-width:600px)) 
    -A space
    -The width of the slot the image will fill when the media condition is true (480px)
  
  Example:  
  "<img
  srcset="elva-fairy-480w.jpg 480w, elva-fairy-800w.jpg 800w"
  sizes="(max-width: 600px) 480px,
         800px"
  src="elva-fairy-800w.jpg"
  alt="Elva dressed as a fairy" />"

  "So, with these attributes in place, the browser will:

    -Look at its device width.
    -Work out which media condition in the sizes list is the first one to be true.
    -Look at the slot size given to that media query.
    -Load the image referenced in the srcset list that has the same size as the slot or, if there isn't one, the first image that is bigger than the chosen slot size.

Sources:

  https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content
  https://css-tricks.com/snippets/css/complete-guide-grid/
  https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images