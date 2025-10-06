# OpenCV.js - Image/Video Processing for Web Frontend

<!--- Currently not available from the publisher -->
<table>
 <tr>
  <td><img src="./Images/2024-OpenCVjs.png"></td>
  <td>
   <p>Satoshi Toyosawa<br/>
    June 2024, Shuwa System, Tokyo, Japan. 408 pages.</p>
   <p><b>Table of Contents</b></p>
    <ul>
     <li>Introdution</li>
     <li>Chapter 1. Basic I/Os - Image, Video and Camera</li>
     <li>Chapter 2. HTML5 User Interfaces</li>
     <li>Chapter 3. Introducing OpenCV.js - Image Processing Library for JavaScript</li>
     <li>Chapter 4. Image Structure</li>
     <li>Chapter 5. Handling Colors</li>
     <li>Chapter 6. Processing images</li>
     <li>Chapter 7. Processing videos</li>
     <li>Appendixes</li>
   </ul>
  </td>
 </tr>
</table>

The Japanese edtion is available from
[Yodobashi](https://www.yodobashi.com/product/100000009003845169/),
[honto](https://honto.jp/netstore/pd-book_33396445.html),
[amazon.co.jp](https://www.amazon.co.jp/dp/4798072168/),
and selected bookstores.


## List of scripts

<!-- 日本語ならこれで取得できる。$ grep '<h1>' *.html | sed 's/:<h1>/` | /g' | sed 's/^/`/' | sed 's/<\/h1>//' | sed 's/&lt;/</' | sed 's/&gt;/>/' -->

Scripts | Description
---|---
`color-background.html` | Replace the background (with luminance adjustment).
`color-binary.html` | Convert to pure black-and-white (0 or 1) image.
`color-gray.html` | Convert to monochorome.
`color-hue.html` | Draw hue colors.
`color-invert.html` | Make negative.
`color-posterize.html` | Posterize.
`color-rgb.html` | Decompose color image to R, G, B monochrome images.
`color-sepia.html` | Make a sepia tone (and more linear filters).
`html-camera.html` | Show video from the camera.
`html-caption.html` | Add subtitles/captions to the video.
`html-frame-chrome.html` | Extract frames from video (for Chrome, Edge, and other major browsers).
`html-frame-firefox.html` | Extract frames from video (for Firefox).
`html-frame-timer.html` | Extract frames periodically from video.
`html-image.html` | Show the image on `<canvas>`.
`html-partial.html` | Copy the sub-region of an image to `<canvas>`.
`html-shuffle.html` | Randomly shuffle video frames.
`html-thumbnail.html` | Generate video thumbnail.
`html-video.html` | Display video.
`img-blur.html` | Blur image.
`img-compose.html` | Image arithmetics (add, subtract, multiply and divide two images).
`img-edge1.html` | Detect edges (contours).
`img-edge2.html` | Draw the edges on the original images.
`img-haarLike.html` | Detect faces (Haar-like features).
`img-hough.html` | Correct tilted document.
`img-morph.html` | Delete the thin lines like power lines in image.
`img-qrcode.html` | Read QR code.
`img-resize1.html` | Demonstrate a various image resizing methods.
`img-resize2.html` | Obfuscate (pixelete) the region of an imagese.
`mat-canvas.html` | Copy `<canvas>` image to `cv.Mat`.
`mat-circle32.html` | Draw a circle by manipulating floating-point Mat.
`mat-circle8.html` | Draw a circle by manipulating 8 bits uint Mat.モノクロで円を描く
`mat-metadata.html` | Print image metadata.
`mat-paint.html` | Create a drawing tool.
`mat-pixel.html` | Determine the closest color name of the given pixel.
`mat-roi.html` | Process only the region of interest (ROI).
`opencv-buildinfo.html` | Show the OpenCV.js build information.
`opencv-consts.html` | Show all the OpenCV.js constants (such as `cv.8UC1`）.
`opencv-cors.html` | Demonstrate CORS error.
`opencv-functions.html` | Show all the OpenCV.js functions.
`opencv-load.html` | Understand the subtle loading timing differences (asynchronous behaviour).
`promise-all.html` | Promisify resouce loading methods.
`promise-event.html` | Promisify events.
`promise-opencv.html` | Promisify OpenCV.js initialization.
`ui-button.html` | Capture video (`<input type="button">`).
`ui-file.html` | Load a local image file(`<input type="file">`).
`ui-options.html` | Select the filter from pulldown menu (`<select>`).
`ui-overlay1.html` | Overlay strings on image. Take 1.
`ui-overlay2.html` | Overlay strings on image. Take 2.
`ui-range.html` | Resize image from trackbar (`<input type="range">`).
`ui-regionselect.html` | Select the region of interest.
`ui-soundonly.html` | Toggle camera on/off (with an Evangelion-like "Sound Only" poster).
`video-add.html` | Overlay the image on video.
`video-flip.html` | Mirror video.
`video-miniture.html` | "Miniaturize" live video (tilt-shift effect).
`video-mog2.html` | Extract forgrond (moving) objects from video.
`video-opticalflow.html` | Detect the motion direction.
`video-transition.html` | Edit two videos with scene transitions (disolve, etc.).
