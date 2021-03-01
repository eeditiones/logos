# E-Editiones logos and design 

## How to embed the E-Editiones logo

There are two ways of embedding the E-Editiones logo on your homepage, as an html image tag importing an SVG file, or entirely as inline SVG.

You can choose from 4 color variations, depending on what fits best to your own layout:  

* `*-color.svg` - color icon and dark font for light backgrounds
* `*-bw.svg` - black/white icon & font for light backgrounds
* `*-color-inverted.svg` - color icon and white font for dark backgrounds
* `*-bw-inverted.svg` - black/white icon & font for dark backgrounds


<p align="center">
<img alt="embed-logo-overview"
src="https://github.com/eeditiones/logos/blob/master/examples/embed-logo-overview.png" />
</p>

[See high resolution PDF with logo overview](examples/embed-logo-overview.pdf)

The images have no background-color included, but if needed, e.g. if the contrast of the original background and the logo colors is too poor, you can apply a suitable background-color for the wrapping `<a>` element.  

The images have no background-color included. If the contrast between the image and your website background is too poor, you can apply a suitable background-color to the wrapping `<a>` element.

The suggested css in the `<a>` element can freely be modified. However, the SVG inline css branding should stay untouched.  

### 1. Using the e-editiones logo SVG file as an `<img>`

Save the SVG file in your project and insert the path in an <img> tag.
Copy and paste the code below and adjust the path to the SVG and possibly also the css of the `<a>` element accordingly.

~~~html
<a href="https://e-editiones.org/" target="_blank" rel="noreferrer" rel="noopener"
  style="
  /* background-color: #fff; */
  display: block;
  /* Adapt the size of the image here, it will preserve its ratio when keeping height to 'auto' */
  width: 190px;
  max-width: 330px;
  height: auto;">

  <img src="path-to-image.svg" alt="Member of e-editiones">

</a>
~~~

### 2. Using the e-editiones logo as “inline” SVG
Instead of importing the svg file in an image tag, you can simply paste the entire code of the SVG files directly into the anchor element.  
 
Just copy the code below and insert the code block into your own html code.
The example below will use the svg image for "Member of E-Editiones", color.

For other images, just replace the SVG block with the content of the wanted SVG file.     
You might need to modify the css inside the `<a>` tag to fit the image correctly into your layout.  


~~~html
<a href="https://e-editiones.org/" target="_blank" rel="noreferrer" rel="noopener"
style="
  display: block;
  background-color: #fff;
  display: block;
  /* set fixed dimensions depending on your layout ... */
  height: auto;
  width: 190px;
  /* ... or leave responsive to fit the available space within a min/max value */
  /* min-width: 133px; */
  /* max-width: 330px; */
  position: relative;
  /* also possible: position:absolute; */
  /* choose position e.g. via auto margin */
  /* margin: 0 0 0 auto; (align right) */
  /* margin: 0; */
  /* choose background color if needed */
  /* background-color: #fff;*/ ">

  <svg> Copy the entire content of the svg file and replace it with this line here...</svg>

</a>
~~~

The full example of an embedded svg file ("Member of E-Editiones", color):

~~~html
<a href="https://e-editiones.org/" target="_blank" rel="noreferrer" rel="noopener"
  style="
  display: block;
  background-color: #fff;
  display: block;
  /* set fixed dimensions depending on your layout ... */
  height: auto;
  width: 190px;
  /* ... or leave responsive to fit the available space within a min/max value */
  /* min-width: 133px; */
  /* max-width: 330px; */
  position: relative;
  /* also possible: position:absolute; */
  /* choose position e.g. via auto margin */
  /* margin: 0 0 0 auto; (align right) */
  /* margin: 0; */
  /* choose background color if needed */
  /* background-color: #fff;*/ ">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 330 127" class="eeditones-logo" role="img"><title>Member of E-Editiones</title><style>.slashes{fill:#f5a623}.eeditiones,.text{fill:#333}</style><path class="slashes" d="M107.052 22l.786.393 1.18-.196c.523.196.785.655.785 1.377l-.196.787.393 1.18v.393l-.59.59h-.393l-.982-.786c0 1.18-.328 1.77-.983 1.77l-.982-.197L97.816 34l-7.271 7.082a5.699 5.699 0 00-1.965 2.36c-.262 0-.787.525-1.573 1.574-1.277.853-2.26 1.902-2.947 3.148-.262 0-1.376 1.115-3.341 3.344l-1.769 2.164c-.36 0-1.146.787-2.358 2.36-.197 0-.524.46-.983 1.378-.655 0-1.048.459-1.179 1.377-.59.393-1.572 1.508-2.948 3.344-.327 0-.655.46-.982 1.377-.557.164-1.277.885-2.162 2.164-.327 0-.982.721-1.965 2.164 0 .295-.786 1.148-2.358 2.557-.098.656-.426.984-.983.984 0 .492-.917 1.803-2.751 3.934-3.472 4.263-9.236 12.197-17.294 23.804-1.801 3.213-3.145 4.507-4.488 5.884L37.878 106H36.5l-.5-1 .5-1.164.395-1.377c.197-.328 1.31-1.443 3.538-3.344.098-.656.294-.984.59-.984l.392.197 11.58-16.346 6.998-8.506c1.408-1.902 2.074-2.886 2.5-3.083 0-.36.344-.994.999-1.42 1.146-1.837 2.062-1.924 2.488-1.924 0-.393-.262-1.115.393-1.377.066-.459 1.703-1.779 4.127-4.205 0-.492.327-.706.982-1 0-.263.959-1.084 2.007-2.002 0-.361.155-.629.941-1.055.295-.754.674-1.39 1.558-1.948 0-.491.452-1.101 1.5-1.79.72-1.311 1.593-1.77 2.052-1.77 1.048-1.541 1.767-2.918 2.947-3.738 0-.46.927-1.463 2.499-2.709 0-.59 1.854-2.315 4.998-5.004 0-.524.083-1.107 1-1.5 0-.394.583-.715 1.5-1.502l12.21-11.711h-.59l1.966-3.541.982-.197zm-1.965 2.95v.591h.197l.196-.59h-.393zm-64.654 78.886v.394l-.393.393v-.393l.393-.394zM93.056 22l.785.389 1.178-.195c.523.195.785.648.785 1.361l-.196.778.392 1.166v.389l-.589.583h-.392l-1.178-1.05c0 1.166-.13 2.022-.785 2.022l-.98-.195-8.154 6.632-7.033 6.967c-.884.616-1.585 1.549-2.01 2.488-.262 0-.722.456-1.507 1.493-1.276.842-2.327 1.988-3.014 3.219-.262 0-1.554 1.047-3.517 3.25l-1.507 2.192c-.36 0-1.302.731-2.512 2.286-.196 0-.547.5-1.004 1.408-.655 0-1.206.67-1.337 1.578-.589.389-1.373 1.171-2.747 2.986-.327 0-.654.585-.981 1.493-.556.162-1.085.727-1.969 1.99-.327 0-1.004.995-2.009 1.99 0 .292-.44 1.095-2.01 2.488-.098.648-.52 1.493-1.077 1.493 0 .486-1.11 1.378-2.941 3.484-3.467 4.211-9.618 12.043-17.664 23.512-1.799 3.175-1.592 4.984-2.933 6.344L23.98 105 23 103.64v-1.361h.785c-.327 0-.523-.26-.589-.778 0-.324 1.112-1.425 3.336-3.304.098-.648.295-.972.589-.972l.392.194 11.775-15.55 6.672-8.358c1.406-1.88 2.322-2.916 2.747-3.11 0-.357.327-.746.981-1.167 1.145-1.814 1.93-2.721 2.355-2.721 0-.389.327-.713.981-.972.066-.454 1.308-1.879 3.729-4.276 0-.486.327-.875.98-1.167 0-.259.524-.842 1.57-1.75 0-.355.393-.744 1.178-1.165.295-.745.883-1.393 1.766-1.944 0-.486.524-1.07 1.57-1.75.72-1.295 1.308-1.943 1.766-1.943 1.047-1.523 2.159-2.69 3.336-3.5 0-.453.785-1.295 2.355-2.526 0-.583 1.57-2.203 4.71-4.86 0-.518.458-.971 1.374-1.36 0-.389.457-.972 1.373-1.75l11.97-11.857h-.588l1.962-3.499.981-.194zm-1.962 2.916v.583h.196l.197-.583h-.393zm-64.562 77.946v.389l-.392.388v-.388l.392-.39z"></path><path class="eeditiones" d="M32.855 56c-.773 0-1.476-.103-2.109-.31C26.25 54.45 24 51.97 24 48.25c0-4.823 3.092-10.404 9.276-16.742C39.461 25.169 45.012 22 49.932 22c1.616 0 2.934.43 3.953 1.292 1.019.861 1.528 1.912 1.528 3.152 0 3.858-2.969 7.544-8.907 11.058-5.939 3.513-10.77 5.27-14.495 5.27-.562 0-1.054-.069-1.475-.207-1.055 1.86-1.582 3.824-1.582 5.89 0 3.584 1.74 5.375 5.218 5.375 3.479 0 7.994-2.308 13.546-6.924 4.287-3.376 7.941-6.959 10.963-10.748.632-.827 1.177-1.24 1.634-1.24.457 0 .685.207.685.62 0 .413-.281.999-.843 1.757-3.795 4.891-8.363 9.232-13.704 13.021C41.112 54.106 36.579 56 32.855 56zm19.923-29.763c0-.827-.896-1.24-2.688-1.24-1.792 0-4.34 1.343-7.643 4.03-4.427 3.583-7.87 7.338-10.33 11.265.421.138.878.206 1.37.206 2.67 0 6.237-1.395 10.7-4.185 4.462-2.79 7.256-5.839 8.38-9.146.14-.344.21-.654.21-.93zM100.139 87.428c0 .572-.366.858-1.097.858H82.339a31.249 31.249 0 00-.182 3.433c0 3.29.777 5.818 2.331 7.585 1.555 1.767 3.764 2.65 6.63 2.65 1.442 0 2.895-.387 4.358-1.164 1.463-.776 2.641-1.767 3.535-2.973l.152-.06c.183 0 .361.112.534.336.173.225.259.49.259.797 0 .43-.65 1.323-1.95 2.682-1.301 1.358-2.713 2.395-4.237 3.11a11.134 11.134 0 01-4.785 1.073c-3.658 0-6.736-1.349-9.235-4.045-2.5-2.697-3.749-6.007-3.749-9.93 0-4.004 1.224-7.396 3.673-10.174 2.448-2.779 5.552-4.168 9.31-4.168 3.15 0 5.797 1.037 7.94 3.11 2.144 2.074 3.216 4.367 3.216 6.88zm-5.547-2.696c0-1.533-.524-2.805-1.57-3.816-1.046-1.011-2.392-1.517-4.038-1.517-1.565 0-2.921.659-4.07 1.977-1.147 1.318-1.924 3.049-2.33 5.194l8.472-.245c1.28-.02 2.19-.143 2.728-.368.538-.224.808-.633.808-1.225zm40.444 18.08c0 .43-.162.665-.487.706-1.159.143-2.5.429-4.024.858-1.523.429-2.712.858-3.565 1.287-.447.225-.773.337-.976.337-.325 0-.487-.163-.487-.49l.243-3.31c-2.153 2.37-4.896 3.555-8.229 3.555-3.515 0-6.507-1.359-8.976-4.076-2.468-2.717-3.703-5.976-3.703-9.776 0-4.311 1.367-7.8 4.1-10.466 2.733-2.666 6.161-4 10.286-4 2.357 0 4.531.736 6.522 2.207V69.44c0-1.655-.203-2.738-.61-3.248-.406-.511-1.34-.848-2.803-1.012-.325-.04-.488-.296-.488-.766 0-.531.163-.797.488-.797 1.91-.45 3.566-.99 4.968-1.624 1.402-.633 2.347-1.195 2.834-1.686.203-.204.417-.306.64-.306.57 0 .854.163.854.49-.325 4.454-.488 8.01-.488 10.665v27c0 1.41.203 2.354.61 2.834.406.48 1.34.823 2.804 1.027.325 0 .487.266.487.797zm-9.296-3.309v-15.69c0-1.063-.614-2.064-1.844-3.004-1.229-.94-2.565-1.41-4.007-1.41-5.934 0-8.9 4.188-8.9 12.565 0 3.31.711 6.058 2.133 8.244 1.423 2.186 3.292 3.279 5.608 3.279 1.321 0 2.52-.301 3.597-.904s2.215-1.63 3.413-3.08zm21.64-32.577c0 .858-.31 1.604-.93 2.237-.62.634-1.366.95-2.24.95-.874 0-1.62-.316-2.24-.95-.62-.633-.93-1.379-.93-2.237 0-.899.305-1.655.915-2.268.61-.613 1.361-.92 2.255-.92.874 0 1.62.307 2.24.92.62.613.93 1.37.93 2.268zm4.267 37.051c0 .572-.163.858-.488.858-.833 0-1.9-.06-3.2-.183-1.463-.123-2.692-.184-3.688-.184a43.52 43.52 0 00-3.657.184c-1.28.122-2.337.183-3.17.183-.325 0-.488-.286-.488-.858 0-.51.163-.786.488-.827 1.727-.225 2.84-.644 3.337-1.257.498-.613.747-1.92.747-3.922V86.63c0-1.634-.208-2.707-.625-3.217-.416-.511-1.325-.848-2.727-1.012-.326 0-.488-.265-.488-.796 0-.49.162-.736.488-.736 2.133-.552 3.88-1.139 5.242-1.762 1.361-.623 2.215-1.14 2.56-1.548.203-.245.427-.367.67-.367.57 0 .854.163.854.49-.325 4.576-.488 8.131-.488 10.665v9.623c0 2.002.25 3.31.747 3.922.498.613 1.63 1.032 3.398 1.257.325.04.488.317.488.827zm21.883-23.536c0 1.103-.264 1.655-.792 1.655l-9.083-.245v14.71c0 3.841 1.362 5.761 4.084 5.761 1.687 0 3.22-.398 4.603-1.195.162 0 .31.108.441.322.133.215.199.444.199.69 0 .51-.757 1.2-2.271 2.068-1.514.869-3.215 1.303-5.105 1.303-2.316 0-4.165-.71-5.547-2.13-1.382-1.42-2.073-3.295-2.073-5.624v-.276l.122-14.894c0-.572-.244-.858-.731-.858h-2.317c-.447 0-.67-.265-.67-.797 0-.408.183-.715.549-.919 2.824-1.675 5.282-4.035 7.375-7.08.224-.326.508-.49.854-.49.569 0 .853.164.853.49l-.244 5.854h8.96c.53 0 .793.552.793 1.655zm13.41-13.515c0 .858-.31 1.604-.929 2.237-.62.634-1.366.95-2.24.95-.874 0-1.62-.316-2.24-.95-.62-.633-.93-1.379-.93-2.237 0-.899.305-1.655.915-2.268.61-.613 1.36-.92 2.255-.92.874 0 1.62.307 2.24.92.62.613.93 1.37.93 2.268zm4.268 37.051c0 .572-.163.858-.488.858-.833 0-1.9-.06-3.2-.183-1.463-.123-2.693-.184-3.688-.184a43.52 43.52 0 00-3.658.184c-1.28.122-2.336.183-3.17.183-.324 0-.487-.286-.487-.858 0-.51.163-.786.488-.827 1.727-.225 2.84-.644 3.337-1.257.498-.613.747-1.92.747-3.922V86.63c0-1.634-.208-2.707-.625-3.217-.417-.511-1.326-.848-2.728-1.012-.325 0-.487-.265-.487-.796 0-.49.162-.736.487-.736 2.134-.552 3.881-1.139 5.242-1.762 1.362-.623 2.215-1.14 2.56-1.548.204-.245.427-.367.671-.367.57 0 .854.163.854.49-.326 4.576-.488 8.131-.488 10.665v9.623c0 2.002.249 3.31.747 3.922.497.613 1.63 1.032 3.398 1.257.325.04.488.317.488.827zM222.57 91.78c0 4.066-1.316 7.411-3.947 10.037-2.632 2.625-6.04 3.938-10.226 3.938-4.185 0-7.599-1.318-10.24-3.954-2.642-2.635-3.963-5.976-3.963-10.02 0-4.107 1.331-7.524 3.993-10.252 2.662-2.728 6.065-4.091 10.21-4.091 4.166 0 7.569 1.358 10.21 4.076 2.642 2.717 3.963 6.14 3.963 10.266zm-6.126-.061c0-3.739-.717-6.727-2.15-8.964-1.432-2.237-3.398-3.356-5.897-3.356-2.479 0-4.44 1.124-5.882 3.371-1.443 2.248-2.164 5.23-2.164 8.949 0 3.698.711 6.635 2.133 8.81 1.423 2.177 3.394 3.264 5.913 3.264 2.52 0 4.49-1.077 5.913-3.233 1.422-2.155 2.134-5.102 2.134-8.841zm41.358 12.258c0 .572-.162.858-.487.858-.813 0-1.809-.06-2.987-.183a37.198 37.198 0 00-3.444-.184c-1.016 0-2.184.061-3.505.184-1.199.122-2.205.183-3.017.183-.326 0-.488-.286-.488-.858 0-.51.162-.786.488-.827 1.402-.164 2.321-.562 2.758-1.195.437-.634.655-1.962.655-3.984V87.735c0-2.288-.447-3.964-1.34-5.026-.895-1.063-2.277-1.594-4.146-1.594-1.178 0-2.22.225-3.124.674-.904.45-1.874 1.247-2.91 2.39v13.792c0 2.022.218 3.35.655 3.984.436.633 1.356 1.031 2.758 1.195.325.04.488.317.488.827 0 .572-.163.858-.488.858-.833 0-1.85-.06-3.048-.183a38.171 38.171 0 00-3.474-.184c-.976 0-2.114.061-3.414.184-1.199.122-2.215.183-3.048.183-.325 0-.487-.286-.487-.858 0-.51.162-.786.487-.827 1.748-.225 2.875-.649 3.383-1.272s.762-1.926.762-3.907V86.63c0-1.634-.208-2.707-.625-3.217-.416-.511-1.346-.848-2.788-1.012-.325 0-.488-.265-.488-.796 0-.49.163-.736.488-.736 2.011-.51 3.688-1.088 5.029-1.731 1.34-.644 2.184-1.17 2.53-1.579.202-.245.426-.367.67-.367.569 0 .853.163.853.49l-.244 3.861c2.926-2.737 5.649-4.106 8.168-4.106 2.764 0 4.923.797 6.477 2.39 1.555 1.594 2.332 3.739 2.332 6.436V97.97c0 2.002.249 3.31.746 3.922.498.613 1.61 1.032 3.338 1.257.325.04.487.317.487.827zm26.608-16.549c0 .572-.366.858-1.097.858H266.61a31.249 31.249 0 00-.183 3.433c0 3.29.777 5.818 2.331 7.585 1.555 1.767 3.764 2.65 6.63 2.65 1.442 0 2.895-.387 4.358-1.164 1.463-.776 2.641-1.767 3.535-2.973l.153-.06c.182 0 .36.112.533.336.173.225.259.49.259.797 0 .43-.65 1.323-1.95 2.682-1.301 1.358-2.713 2.395-4.237 3.11a11.134 11.134 0 01-4.785 1.073c-3.658 0-6.736-1.349-9.235-4.045-2.5-2.697-3.749-6.007-3.749-9.93 0-4.004 1.224-7.396 3.673-10.174 2.448-2.779 5.552-4.168 9.31-4.168 3.15 0 5.797 1.037 7.94 3.11 2.144 2.074 3.216 4.367 3.216 6.88zm-5.547-2.696c0-1.533-.523-2.805-1.57-3.816-1.046-1.011-2.392-1.517-4.038-1.517-1.565 0-2.921.659-4.069 1.977-1.148 1.318-1.925 3.049-2.332 5.194l8.473-.245c1.28-.02 2.19-.143 2.728-.368.539-.224.808-.633.808-1.225zM308 96.929c0 2.492-.975 4.586-2.926 6.282-1.95 1.696-4.307 2.544-7.07 2.544-.976 0-2.48-.215-4.512-.644-1.524-.306-2.56-.46-3.108-.46-.163-1.43-.539-3.605-1.128-6.527 0-.307.295-.46.884-.46.487 0 .782.164.884.49.467 1.512 1.391 2.83 2.773 3.954 1.382 1.124 2.804 1.685 4.267 1.685 1.524 0 2.708-.418 3.55-1.256.844-.838 1.266-2.012 1.266-3.524 0-.96-.35-1.808-1.052-2.544-.7-.735-2.22-1.645-4.556-2.727-3.068-1.41-5.095-2.738-6.08-3.985-.986-1.246-1.479-2.737-1.479-4.474 0-2.145.925-3.989 2.774-5.532 1.849-1.542 4.033-2.313 6.552-2.313 1.057 0 2.54.184 4.45.551 1.057.205 1.748.307 2.073.307.06 2.41.193 4.464.396 6.16 0 .306-.295.46-.884.46-.508 0-.792-.164-.853-.49-.224-1.492-.783-2.703-1.677-3.633-.894-.93-1.96-1.394-3.2-1.394-3.17 0-4.754 1.39-4.754 4.168 0 .94.375 1.808 1.127 2.605.752.797 2.388 1.828 4.907 3.095 3.007 1.512 4.989 2.82 5.944 3.923.955 1.103 1.432 2.35 1.432 3.739z" fill="#000"></path><path class="text" d="M164.68 23.07l3.004 8.45 3.199-8.45h1.61V38h-1.2v-6.614l.092-6.675-3.312 8.798h-.8l-3.076-8.655.103 6.532V38h-1.2V23.07h1.58zm21.526 15.135c-.772 0-1.477-.143-2.112-.43a5 5 0 01-1.636-1.17 5.259 5.259 0 01-1.056-1.727 6.066 6.066 0 01-.384-2.107v-.441a6.417 6.417 0 01.394-2.215 5.713 5.713 0 011.051-1.784 4.912 4.912 0 011.57-1.195 4.398 4.398 0 011.937-.436c.738 0 1.391.133 1.959.4.567.267 1.044.63 1.43 1.092.386.462.68 1 .882 1.615.202.615.306 1.275.313 1.98v.748h-8.306v.236c.007.58.106 1.136.297 1.666.192.53.462.996.81 1.4.35.403.77.726 1.262.968a3.66 3.66 0 001.64.364c.684.007 1.303-.12 1.856-.379a3.896 3.896 0 001.415-1.128l.78.585a4.546 4.546 0 01-1.667 1.415c-.345.17-.723.304-1.133.4-.41.095-.844.143-1.302.143zm-.236-10.459a3.305 3.305 0 00-2.471 1.067c-.314.334-.574.73-.78 1.184a5.43 5.43 0 00-.42 1.492h7.024v-.134a4.374 4.374 0 00-.251-1.338 3.656 3.656 0 00-.656-1.153 3.251 3.251 0 00-1.041-.81c-.41-.205-.878-.308-1.405-.308zm13.642-.84l.03 1.24c.226-.43.535-.778.929-1.04.393-.264.89-.399 1.492-.406.314 0 .593.036.835.108.243.072.453.172.63.302.179.13.329.286.452.467.123.181.222.378.297.59.233-.417.552-.764.96-1.041.406-.277.913-.419 1.522-.426.478 0 .878.082 1.2.246.32.164.58.387.779.667.198.28.34.605.425.974.086.37.129.759.129 1.169l-.01 8.244h-1.15l-.01-8.244c0-.24-.023-.479-.071-.718a1.916 1.916 0 00-.251-.646 1.313 1.313 0 00-.503-.461c-.215-.117-.49-.171-.825-.164-.342.006-.63.061-.867.164a1.738 1.738 0 00-.943.948 3.14 3.14 0 00-.19.61l-.01 8.511h-1.149l-.01-8.357c0-.232-.024-.461-.072-.687a1.705 1.705 0 00-.25-.605 1.307 1.307 0 00-.498-.43c-.212-.11-.482-.161-.81-.154a2.293 2.293 0 00-.836.153c-.229.096-.42.224-.574.385-.154.16-.277.345-.37.554a3.84 3.84 0 00-.22.65l-.01 8.491h-1.159V26.905h1.108zm27.074 5.66c0 .717-.087 1.416-.261 2.096a5.628 5.628 0 01-.8 1.805 4.17 4.17 0 01-1.359 1.261c-.547.318-1.196.477-1.948.477a4.24 4.24 0 01-1.933-.436 3.934 3.934 0 01-1.45-1.256L218.882 38h-1.149V22.25h1.23v6.204a4.01 4.01 0 011.41-1.292c.565-.308 1.206-.462 1.923-.462.76 0 1.415.156 1.97.467a3.989 3.989 0 011.363 1.25c.355.524.62 1.125.795 1.805.174.68.261 1.39.261 2.128v.215zm-1.24-.216c0-.554-.059-1.104-.175-1.65a4.775 4.775 0 00-.564-1.472 3.107 3.107 0 00-1.04-1.056c-.435-.27-.97-.405-1.605-.405a3.193 3.193 0 00-2.605 1.307c-.198.27-.362.562-.492.877v5.178c.137.3.31.576.518.825.208.25.447.462.717.636a3.45 3.45 0 001.882.549c.622 0 1.147-.134 1.574-.4a3.14 3.14 0 001.036-1.051c.263-.434.454-.925.574-1.472.12-.547.18-1.097.18-1.65v-.216zm15.066 5.855c-.772 0-1.476-.143-2.112-.43a5 5 0 01-1.636-1.17 5.259 5.259 0 01-1.056-1.727 6.066 6.066 0 01-.384-2.107v-.441a6.417 6.417 0 01.395-2.215 5.713 5.713 0 011.05-1.784 4.912 4.912 0 011.57-1.195 4.398 4.398 0 011.937-.436c.739 0 1.391.133 1.959.4.567.267 1.044.63 1.43 1.092.387.462.68 1 .882 1.615.202.615.306 1.275.313 1.98v.748h-8.306v.236c.007.58.106 1.136.298 1.666.191.53.461.996.81 1.4.348.403.769.726 1.26.968a3.66 3.66 0 001.641.364c.684.007 1.303-.12 1.856-.379a3.896 3.896 0 001.415-1.128l.78.585a4.546 4.546 0 01-1.666 1.415c-.346.17-.723.304-1.134.4-.41.095-.844.143-1.302.143zm-.236-10.459a3.305 3.305 0 00-2.47 1.067c-.315.334-.575.73-.78 1.184a5.43 5.43 0 00-.42 1.492h7.023v-.134a4.374 4.374 0 00-.25-1.338 3.656 3.656 0 00-.657-1.153 3.251 3.251 0 00-1.04-.81c-.411-.205-.88-.308-1.406-.308zM261.22 26.7a7.6 7.6 0 01.923.057c.307.037.564.09.769.159l-.154 1.179a9.428 9.428 0 00-.861-.144 7.455 7.455 0 00-.882-.051c-1.04 0-1.921.246-2.646.738-.724.492-1.234 1.248-1.528 2.266l.01 7.096h-1.27V26.905h1.178l.082 1.928v.226a4.914 4.914 0 011.795-1.728c.745-.42 1.606-.63 2.584-.63zM280.129 32.289a6.934 6.934 0 01.349-2.143 5.49 5.49 0 01.969-1.78c.42-.509.936-.914 1.548-1.215.612-.3 1.304-.45 2.076-.45.78 0 1.475.15 2.087.45.612.301 1.13.706 1.553 1.215.424.51.749 1.103.975 1.78.225.676.341 1.39.348 2.143v.338a7.035 7.035 0 01-.343 2.143 5.365 5.365 0 01-.97 1.78 4.64 4.64 0 01-1.548 1.209c-.608.297-1.302.446-2.081.446-.78 0-1.475-.149-2.087-.446a4.624 4.624 0 01-1.553-1.21 5.438 5.438 0 01-.974-1.779 6.934 6.934 0 01-.35-2.143v-.338zm1.23.338c0 .588.082 1.155.246 1.702a4.61 4.61 0 00.718 1.451c.315.42.703.757 1.164 1.01.461.253.996.38 1.605.38.601 0 1.133-.127 1.594-.38.462-.253.848-.59 1.159-1.01.311-.42.549-.904.713-1.45a5.891 5.891 0 00.246-1.703v-.338c0-.581-.082-1.145-.246-1.692a4.61 4.61 0 00-.718-1.451 3.633 3.633 0 00-1.17-1.015c-.464-.257-.997-.385-1.599-.385-.601 0-1.133.128-1.594.385a3.597 3.597 0 00-1.159 1.015c-.31.42-.548.904-.713 1.45a5.856 5.856 0 00-.246 1.693v.338zm26.07-4.717h-4.42l.02 10.09h-1.27l.01-10.09h-3.025v-1.005h3.035v-.882c.007-.758.125-1.398.354-1.917.229-.52.54-.942.933-1.266a3.584 3.584 0 011.374-.698 6.455 6.455 0 011.676-.21c.39 0 .77.024 1.138.072.37.048.746.116 1.128.205l-.153 1.046a8.35 8.35 0 00-.934-.185A7.468 7.468 0 00306.24 23c-.444 0-.86.047-1.246.143a2.691 2.691 0 00-1.02.487 2.338 2.338 0 00-.697.928c-.171.39-.26.879-.267 1.466v.882h4.42v1.005z"></path></svg>
</a>
~~~
