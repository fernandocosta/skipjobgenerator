<style>
  body {
    background: #2f343d
  }

  .bubble {
    background: white;
    color: white;
    border-radius: 8px;
    padding: 1em;
    position: absolute;
    top: 50%;
    left: 50%;
    margin-right: -50%;
    transform: translate(-50%, -50%);
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Meiryo UI', Arial, sans-serif;
    
  }

  .texxt {
    ttom-color:
rgb(68, 68, 68)
;
initiala, abbr, acronym, address, applet, article, aside, audio, b, big, blockquote, body, canvas, caption, center, cite, code, dd, del, details, dfn, div, dl, dt, em, embed, fieldset, figcaption, figure, footer, form, h1, h2, h3, h4, h5, h6, header, hgroup, html, i, iframe, img, ins, kbd, label, legend, li, mark, menu, nav, object, ol, output, p, pre, q, ruby, s, samp, section, small, span, strike, strong, sub, summary, sup, table, tbody, td, tfoot, th, thead, time, tr, tt, u, ul, var, video
border-bottom-style:
solid
;
border-bottom-width:
0px
;
border-image-outset:
0px
;
border-image-repeat:
stretch
;
border-image-slice:
100%
;
border-image-source:
none
;
border-image-width:
1
;
border-left-color:
rgb(68, 68, 68)
;
border-left-style:
solid
;
border-left-width:
0px
;
border-right-color:
rgb(68, 68, 68)
;
border-right-style:
solid
;
border-right-width:
0px
;
border-top-color:
rgb(68, 68, 68)
;
border-top-style:
solid
;
border-top-width:
0px
;
box-sizing:
border-box
;
color:
rgb(68, 68, 68)
;
display:
block
;
font-family:
-apple-system, system-ui, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Helvetica Neue", "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Meiryo UI", Arial, sans-serif
;
font-size:
14px
;
height:
20px
;
line-height:
20px
;
list-style-image:
none
;
list-style-position:
outside
;
list-style-type:
none
;
margin-bottom:
0px
;
margin-left:
0px
;
margin-right:
0px
;
margin-top:
0px
;
opacity:
1
;
overflow-wrap:
break-word
;
padding-bottom:
0px
;
padding-left:
0px
;
padding-right:
0px
;
padding-top:
0px
;
text-align:
left
;
transition-delay:
0s
;
transition-duration:
1s
;
transition-property:
opacity
;
transition-timing-function:
linear
;
unicode-bidi:
isolate
;
user-select:
text
;
vertical-align:
baseline
;
width:
403px
;
-webkit-box-direction:
normal
;
-webkit-
  }

  .mention-link {
    
    color:
      rgba(29, 116, 245, 0.2);
    border-bottom-color:
      rgb(19, 103, 154);
    border-bottom-style:
      solid;
    border-bottom-width:
      0px;
    border-image-outset:
      0px;
    border-image-repeat:
      stretch;
    border-image-slice:
      100%;
    border-image-source:
      none;
    border-image-width:
      1;
    border-left-color:
      rgb(19, 103, 154);
    border-left-style:
      solid;
    border-left-width:
      0px;
    border-right-color:
      rgb(19, 103, 154);
    border-right-style:
      solid;
    border-right-width:
      0px;
    border-top-color:
      rgb(19, 103, 154);
    border-top-style:
      solid;
    border-top-width:
      0px;
    box-sizing:
      border-box;
    color:
      rgb(19, 103, 154);
    cursor:
      pointer;
    display:
      inline;
    font-family:
      -apple-system, system-ui, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Helvetica Neue", "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Meiryo UI", Arial, sans-serif;
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    Oxygen,
    Ubuntu,
    Cantarell,
    'Helvetica Neue',
    'Apple Color Emoji',
    'Segoe UI Emoji',
    'Segoe UI Symbol',
    'Meiryo UI',
    Arial,
    sans-serif.global-font-family font-size:
      14px;
    font-weight:
      700;
    height:
      auto;
    line-height:
      20px;
    list-style-image:
      none;
    list-style-position:
      outside;
    list-style-type:
      none;
    margin-bottom:
      0px;
    margin-left:
      0px;
    margin-right:
      0px;
    margin-top:
      0px;
    overflow-wrap:
      break-word;
    padding-bottom:
      2px;
    padding-left:
      4px;
    padding-right:
      4px;
    padding-top:
      0px;
    text-align:
      left;
    text-decoration-color:
      rgb(19, 103, 154);
    text-decoration-line:
      none;
    text-decoration-style:
      solid;
    user-select:
      text;
    vertical-align:
      baseline;
    width:
      auto;
    -webkit-box-direction:
      normal;
    -webkit-f
  }
</style>
<div class="bubble">
    <div class="texxt">
    <a class="mention-link" id = 'nickname' title=""></a>
      <span id ='message'></span>
    </div>
  </div>
<script>
  var reasons = [
    'Отсутствую по причине болезни',
    'Заболел',
    'Сикдей',
    'Отсутствую по семейным обстоятельствам',
    'Отсутствую',
    'Болею',
  ];
  var date = new Date();
  var day = date.getDate()>=10 ? date.getDate():'0'+date.getDate();
  var month = date.getMonth()>=10 ? date.getMonth():'0'+date.getMonth();
  var reason = reasons[Math.floor(Math.random()*reasons.length)];
document.querySelector('#message').innerHTML = day+'/'+month+' '+reason;
document.querySelector('#nickname').innerHTML = location.hash.replace('#','@');
</script>
