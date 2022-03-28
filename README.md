# cpnt-262-a7
### Will Tengyuan Li
### Plans
- create a reuseable card component including title, text, cta image, tags.
- set props to pass information.
- use v-if render a taglist.
- add arrayof object to card.
### Todos
- I created a card component. added 5 divs. each one contains image, title,text,tag,cta.
- The information of each div will be passed from the parent page which is TheBody by PROPS.
- I used v-if on the line 12 in TheCard.vue. I have tags in the 1st and the 2nd card. but I don't have tag in the 3rd card.
### problems
- when I was trying to pass information by using props. I couldn't get that work.
- I asked my friend Spark. He explain me how that work.
  - The prop is used to pass in an initial value; the child component wants to use it as a local data property afterwards.
  - The prop is passed in as a raw value that needs to be transformed.
- I still a little confused, but Spark helped me out with the rendering part.
- I think I need more practice and more understanding.