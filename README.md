#### Button Styling

Here are some of the disadvantages of my approach. I have also included a few revisions I would like to make to my process in the future:

  - Eyeballing the styling of the button on the template, which led to an inaccurate configuration of gradients and shadowing. For example, I tried to account for the heavier gray component of the gradient on the button half of the button by generating a larger inset box shadow, which did not work effectively.

  - I also attempted to use a CSS produced symbol to generate the arrow on the button. This arrow is not very formattable and while I was able to scale it down using `font-size: smaller`, I was unable to make it more narrow to mimic the template. If I attempted this exercise again, I would try to get a more scaled version of the arrow that would easier to format without needing to change specific dimensions.

  - Finally, from a reusability standpoint, this button is fairly hardcoded and would be hard to use out of the box in other applications. From a styling standpoint, I would pull out a lot of the constant colors, spacings, etc. and place them in a dedicated `_styling_constants.scss` partial file. I would also make this button a React class that would take params and would more easily generate the styled button.

#### Feature Breakdown

mockup 1: M1, mockup 2: M2

What are the most important questions you have about the mocks and how they should work?

  - M1 & M2: For data flow across the app, is there an API connected to the frontend that provides this? What are the security requirements to establish that connection (JWT, basic auth, etc.)? How is data formatted and expected to be sent back?

  - M1 & M2: What does the mobile counterpart for these mockups look like?

  - M1 & M2: Are there common UI elements on these mockups that can be generated from an existing standardized company (or established 3rd party) library? What are the exact color schemes that need to used, to match with company established standards?

  - M1 & M2: Is there a preexisting library used to handle mapping the room iframe? What are the exact requirements of navigating the room on the iframe? On what basis are the '+' points populated on the iframe? How are these items identified? Will the identification mechanism change in the future? Where does the data for these items come from? Is there an a mockup to to handle when a failed data call is made?

  - M1: What does the toggle button by the 'Your Living Room Concept' title do?

  - M1: How does the progress bar for the timeline at the top of the mockup get populated? What defines how much its populated?

What seems like, potentially, the biggest unknown?

  - Generating a dynamic iframe that can be populated with different schematics so that it does not have to be updated constantly to handle changing technologies. Additionally, how is the correct data linked to the correct item in the room? Is that hardcoded in an API call? How will that change in the future?

What changes would you recommend making to make this interface work well on mobile?

  - Generating mockups of rooms using panoramic pictures and then simulating new items in real time (right on the phone) from a preexisting plan, superimposed onto the iframe would be more engaging to the mobile user.
