*Five main features of sass:
  1. Variable  $bg_color
  2. Nested
  3. Reuse code
        @mixin left_image() {
        float: left;
        width: 100px;
        margin-right: 20px;
      }
      .cart {
        width: 900px;
        margin: auto;
        background: $bg_color;
        img {
          @include left-image;
        }
      }
      .shop {
        width: 600px;
        margin: auto;
        img {
          @include left_image;
        }
      }\
  4. Pseudo class (:hover, :active, :link...)
    h1{
      ...
      &:hover{

      }
      &===take id of parent element(here is h1)
    }

  5. Calculation feature
  width: ($height_content - (2*$space))/3;

*npm run compile:sass
<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-plus-circle" viewBox="0 0 16 16">
  <path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/>
  <path d="M8 4a.5.5 0 0 1 .5.5v3h3a.5.5 0 0 1 0 1h-3v3a.5.5 0 0 1-1 0v-3h-3a.5.5 0 0 1 0-1h3v-3A.5.5 0 0 1 8 4z"/>
</svg>


@use'../custom' as *; to customize

*nest feature:
  .class_name{
    child1{

    }
    child2{
      
    }
  }

*line-height  is the same to padding top

*copy color to manypixel website to create art illustration
*text-end or text-start 
*getwave.io
*glightbox to display popup video

*shadow-sm

*h1.display-3(custom).fw-

*use -webkit to create text with gradient background color
    &--title{
        font-size:1.8rem;
        text-transform: capitalize;
        font-weight: 600;
        font-family: 'Poppins', sans-serif;
        display:inline-block;
        background-image: linear-gradient(to right, $primary, $secondary);
        background-clip: text;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        
*d-block to xuong dong.

*overflow-hidden: hide the part dose not stay inside of div

*change before of list to check notation:
  li::before{
            font-family: "Font Awesome 5 Free";
            content: "\f00c";
            font-weight: 600;
            margin-right: 0.5rem;
            font-size: 1.2rem;
        }