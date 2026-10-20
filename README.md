Author: Nova Wolta

Purpose: Work for the COMP1B Course, learning CSS box models.

Records: Checking if CSS file is linked, adding color to p element

Added color and it worked as desired.

Added class for article card.

Expected: content-box

    Content width is set at 240px | content width is 240px

    Border-box width:
     Width is set at 240px but content is placed outside of this width causing the padding and border to get added to this "content width", the padding is 16px and including the two padding edges this becomes 32px; the border is 2px and taking the two border edges this becomes 4px. adding both totals after the two values for the border and padding to get: 240px + 32px + 4px = 276px | padding is 16px but border is showing different, 1.6px [seems to be a browser issuse]

    Total horizontal footprint:
     add the 12px margin twice to the Border-box width to find the total horizontal footprint, 276px + 24px = 300px | due to the border change the acutal footprint is a little different from what is coded.

Expected: border-box

    Content width is set to 240px but because the content is fixed inside the declared padding and border values the set 16px (32px for both sides) for padding and the set 2px (4px for both sides) for the border get subtracted causing a value of 204px | the acutal is a little off due to the afore mentioned border problem coming in at a 204.8px

    Border-box width:
     The widith is set to 240px | width is 240px

    Total horizontal footprint:
     The border-box width gets added to the left and right margin of 12px for a total of 24px being added the border-box: 240px +  24px = 264px | the readings match the 240px + 24px

Differnece between inline, inline-block, and block: My noticed changes where how inline seems to be more of a felx to the contents of the line where as any of the "block" displays make the border stick to the invisible border of the text.


Card width changing the view ports - 
at 375px, it is supposed to be 310px but due to border issuses its coming in at a 309.6px
at 1024px it is 590.4px and I'm lead to belive it's supposed to be 590.8px

When wanting a element in HTML to felx to fit different veiw ports having a 100% width and using display declarations are a great tool. The margin is outside of the content, padding and border; because of this, margin is outside of width declarations. Border-box in a content-box is a combination of width, padding, and border and in border-box border-boxes it's just plain width.

# comp1b-m02-activity
