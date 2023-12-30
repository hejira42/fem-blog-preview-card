Here you go. The biggest problems are caused by height 100vh and px font size. Other items are just suggestions really 

Link fonts in html head instead of css imports. It's better for performance
NEVER write font size in px. Not even once. I've written about why on https://fedmentor.dev/
Never limit the height of elements that contain text, including the body. Use min-height 100vh not height
Max width needs to be in rem not px
You can't use overflow hidden on this card or it cuts off the shadow. It's not needed anyway
The tag must not have  an explicit width. Think about what happens when a blog has a tag with a longer word! Just like with buttons use padding not heights and widths
Make sure with font sizes you're picking intentional rem values not just rounding. It's unusual to see font sizes with rems at only 1 decimal place tbh
Use gap with flex not side margins on its children
The avatar image can have an explicit height and width instead of max width
Really important - include a modern css reset at the start of the styles in every project. This needs to set img elements as display block and max-width 100% amongst other things
