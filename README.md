<img src="assets/images/bean.png" style="margin: 0;height:20%;width:20%">

# BeenThere
<b>Problem Statement</b><br>
We live in the age of customisation where people want to curate different offerings or products all of the time. They would love to curate their own holiday
so it does not feel like a stale package holiday from the 70s. They do not have the local knowledge when they visit a new place to know all the best places to go to and 
what places to visit. 

<br><br>
<b>Proposed Solution</b><br>
<i>BeenThere</i> is a website aimed at curating customisable holidays based on the invaluable knowledge of the locals. They know the best
hotels,restaurants and bars to go to, as they have been living there for at least four years. The locals are carefully selected by the BeenThere team and usually have a background in the
hospitality industry or the food industry. 

## UX
The user experience for the website is aimed at providing users the ability to make their first attempt at looking where they want to travel to and looking for what hotels are available, in the city that they want to book in.
As they look at the google maps functionality provided they might then make the decision to actually have a local curate their trip for them, as they look at the five main city destinations and read about the locals who are designing the curated trips this month. 

<b>User Story 1: Be Inspired</b><br>
- A new user comes across the <b>BeenThere</b> website when starting to plan their holiday. They do not know where they want to go on holiday yet and would like to be inspired by the 5, monthly cities with the current 3 recommendations for hotels, bars, and restaurants.


<b>User Story 2: Checking which cities are in focus this month and just using the hotel finder</b><br>
- As a new or experienced user, the user checks which 5 cities are in focus for the <b>BeenThere</b> team this month, and if they do not want to use the curated trip part of the website, they may choose to use the specialised google map and search functionality from the <b>BeenThere</b> website as
the map has filtered out most items from it, that does not relate to holiday planning, to choose their hotel and plan their trip.<br><br>

<b>User Story 3: Booking flight post trip planning</b><br>
- After a user has booked their curated trip; They are brought to a 'thank you' page which sets expectations with them that they can expect their curated trip within 48 hours and that they can go ahead and book their flight. 
The booking of the flight is quickly started through the skyscanner widget on the <b>BeenThere</b> website as it is convenient for the user to get the flight booking out of the way.<br><br>


## Features
1) <b>Custom google maps for highlighted cities</b><br><br> 
Users are able to look for curated trips on a specific city page that include a specially filtered google map that only includes the items that you would need for planning a holiday. This map also includes 3 markers that include the suggestions from the local for the hotel, restaurant and bar that they have
chosen to highlight this month. The markers have even-listeners built in so that when the user clicks on the marker they can read a blurb about the location and also see what it looks like in the picture provided.

2) <b>Request to book form</b><br><br> 
After the user has succesfully chosen the city they want to travel to, they can press the 'book your trip' button which brings them to the 'request to book form'
which allows them to highlight all of their choices and requirements for their trip to the <b>BeenThere</b> team so that they have all of the information to plan the trip for the user. The user then presses the 'Submit Request for Ideal Holiday' button which has an
event-listener on it that then thanks them as it loads the next page.

3) <b>Hotel Search google map with search bar</b><br><br> 
Users are able to filter the country to the current countries which are in focus this month for the <b>BeenThere</b> team, this will centre the google map on the country in question. The user can then type in the city that they want to book in, this does not have to be part of the cities in focus and it will centre the map on the city they searched for and bring up all of the hotels in the centre of the city.
There is a semi-transparent list type table that they can see as well that lists all of the hotels so that they can quickly have a read through rather than looking at all of the hotels that are distributed on the map. The hotels are labelled with the letters of the alphabet so that the user
can remember which hotel they have already reviewed and can match the letters to the hotel that they can see in the transparent list. If the user clicks on the individual markers for the hotels it will bring up information about the hotel so that the user can book the hotel and also visit the hotel's own website. If they choose not to look at the list and just click on the hotels on the actual map I have built in an event-listener that allows them to hide this semi-tranparent list by pressing the 'hide the search table' button below. 

4) <b>SkyScanner flight booking widget</b><br><br> 
After the user requests to book their trip they are brought to a 'post booking' that educates the user that it will take around 48 hours for them to receive their curated trip, underneath that education the user is 'called to action' to book their flight using the
skyscanner widget that is built into that page. It allows the user to choose if they want to book a return, one-way or multi-city ticket, where the flight is going to and coming from, it allows the user to choose the day they want to depart and the day they want to return,
how many adults and children are going and then what class of flight ticket they want to book. They then press the 'search flights' button which brings them to the skyscanner page with the live flight information. The link has a unique referal code built into it though that we will get referral comission on.


###Future Feature Ideas
- I had an idea for using iframes to display the information from different websites on another page as a tool; For example you could have yahoo finance, trading view, and tastyworks open on the same website page. They don't support iframes though so I would probably try and scrape the information using beautifulsoup and python at a later stage.
- The quick-links section was originally on every page but then I decided against this because it actually encourages people to leave the website. I left it in on the trading ideas page as it becomes useful as a lot of the information on the page would be directly from those websites. Once there are multiple posts on the 'trade ideas' blog it might be worth making the icon links specific to the stock ticker from the post and having multiple of these quick-links icon groups. 
- Once there are more posts on the trade ideas page it might be worth implementing some of the bootstrap pagenation features to focus the users attention more, rather than them scrolling down for a long time to find the section they want and getting disctracted by the passing-other-posts.


## Technologies Used

- [Bootstrap](https://getbootstrap.com/)
    - The project uses **Bootstrap** to speed up the HTML and CSS work.

- [Google Fonts](https://fonts.google.com/)
        - I used archivo as this website is a little bit like an archive of recommended content and ideas. It looks very strong and clean as well as a font.

- [CSS](https://cssreference.io/)

- [Font Awesome](https://fontawesome.com/) 
        - 'fa fa-graduation-cap' - 'fa fa-facebook' - 'fa fa-twitter' - 'fa fa-instagram'

- [Google Maps API](https://developers.google.com/maps/documentation/javascript/tutorial)
        - I used the google maps api to make the custom google maps to filter out all of the noise of the google maps and to leave just the points of interest for holiday planning.
        - The custom markers and pop-up window for the recommended hotel, restaurant and bar were made using google maps api.

- [Google Places API](https://developers.google.com/places/web-service/intro)
        - I used the google places api to create a map and search bar that specifically lets you filter a country, type in a city, and the map then displays all of the hotels in that city.
        - The map also shows a transparent list with the hotel labels so that a user can see quickly where a hotel is located. I built a button that can make this list invisible if the user wishes to concentrate just on the map.
        - The markers of the hotels on the map lets you also click on them and display more information such as name of hotel, website url, and phone number.






## Testing
<b>Testing Summary</b><br>


1. <b>User Story 1:</b> Be Inspired: index.html page.
    1. Try to read all of the text on the index page and make sure that the text looks strong. - Success
    2. The image loads. - Success
    3. Try the 'Curated Trip' button and see if it displays 'choose' and 'city buttons' section. - Success
    4. Try the 'Search for Hotels' button and see if it displays the map and the search bar. - Success
    5. Try entering a city into the search bar and see if the map responds. - Success
    6. Check if the semi-transparent hotel list is there. - Success
    7. Try the 'Hide Search Table' button and see if the hotel list becomes invisible.  - Success
    8. Try moving the map around with hand cursor. - Success
        - Found Social Media buttons floating in the map. I don't want the user going to social media when they are searching for hotels so I just added an event listener to make the social media buttons disappear when the hotels button is pressed.      
    9. Try the 'Podcasts' button and hover-over response in the dropdown menu for narrower screens. - Success
    10. Try the 'Trade Ideas' button and hover-over response in the dropdown menu for narrower screens. - Success
    11. Try the 'Contact Us' button and hover-over response in the dropdown menu for narrower screens. - Success
    12. Try the 'facebook' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    13. Try the 'twitter' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    14. Try the 'instagram' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    15. Check the index.html page in responsinator:<a href="https://www.responsinator.com/?url=https%3A%2F%2Fsammckenna1986.github.io%2Fmilestone_project_1-static_frontend%2Findex.html"></a>
        - iPhone eXpensive portrait · width: 375px - Success
        - iPhone eXpensive landscape · width: 734px - Success
        - Android (Pixel 2) portrait · width: 412px - Success
        - Android (Pixel 2) landscape · width: 684px - Success
        - iPhone 6-8 portrait · width: 375px - Success
        - iPhone 6-8 landscape · width: 667px - Success
        - iPhone 6-8 Plump portrait · width: 414px - Success
        - iPhone 6-8 Plump landscape · width: 736px - Success
        - iPad portrait · width: 768px - Success (1. There is a lot of white space at the bottom but I am actually fine with it as it draws the eye more towards the social links and it is unusual so it does not have the 'wall paper' effect on people. 2. I tried another picture underneat but it looked too busy.)
        - iPad landscape · width: 1024px - Success (1. There is a lot of white space at the bottom but I am actually fine with it as it draws the eye more towards the social links and it is unusual so it does not have the 'wall paper' effect on people. 2. I tried another picture underneat but it looked too busy.)
    
2. <b>User Story 2:</b> Looking for quick book recommendations: reading.html page.
    1. Try to read all of the text on the 'reading' page, make sure that the information is correct, and make sure that the text looks strong. - Success
    2. The background image now loads faster as I replaced the jpg files with the converted png files. - Success
    3. Try the 'Your Own Money Investments' link in the logo  - Success
    4. Try the 'Reading' button and hover-over response in the navbar. - Success
    5. Try the 'Podcasts' button and hover-over response in the navbar. - Success
    6. Try the 'Trade Ideas' button and hover-over response in the navbar. - Success
    7. Try the 'Contact Us' button and hover-over response in the navbar. - Success
    8. Try the 'Reading' button and hover-over response in the dropdown menu for narrower screens. - Success
    9. Try the 'Podcasts' button and hover-over response in the dropdown menu for narrower screens. - Success
    10. Try the 'Trade Ideas' button and hover-over response in the dropdown menu for narrower screens. - Success
    11. Try the 'Contact Us' button and hover-over response in the dropdown menu for narrower screens. - Success
    12. Try the 'facebook' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    13. Try the 'twitter' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    14. Try the 'instagram' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    15. Try the 'One Good Trade' link in the book title, and hover-over response in the books section. - Success
    16. Try the 'Market Wizards' link in the book title, and hover-over response in the books section. - Success
    17. Try the 'How I Made $2,000,000 in the Stock Market' link in the book title, and hover-over response in the books section. - Success
    18. Try the 'Top 10 Trading Setups' link in the book title, and hover-over response in the books section. - Success
    19. Check the index.html page in responsinator: <a href="https://www.responsinator.com/?url=https%3A%2F%2Fsammckenna1986.github.io%2Fmilestone_project_1-static_frontend%2Freading.html"></a>
    - iPhone eXpensive portrait · width: 375px - Success
    - iPhone eXpensive landscape · width: 734px - Success
    - Android (Pixel 2) portrait · width: 412px - Success
    - Android (Pixel 2) landscape · width: 684px - Success
    - iPhone 6-8 portrait · width: 375px - Success
    - iPhone 6-8 landscape · width: 667px - Success
    - iPhone 6-8 Plump portrait · width: 414px - Success
    - iPhone 6-8 Plump landscape · width: 736px - Success
    - iPad portrait · width: 768px - Success (ipad looks great)
    - iPad landscape · width: 1024px - Success (ipad looks great)


3. <b>User Story 3:</b> Looking for quick podcast recommendations: podcasts.html page.
    1. Try to read all of the text on the 'podcasts' page, make sure that the information is correct, and make sure that the text looks strong. - Success
    2. The background image now loads faster as I replaced the jpg files with the converted png files. - Success
    3. Try the 'Your Own Money Investments' link in the logo  - Success
    4. Try the 'Reading' button and hover-over response in the navbar. - Success
    5. Try the 'Podcasts' button and hover-over response in the navbar. - Success
    6. Try the 'Trade Ideas' button and hover-over response in the navbar. - Success
    7. Try the 'Contact Us' button and hover-over response in the navbar. - Success
    8. Try the 'Reading' button and hover-over response in the dropdown menu for narrower screens. - Success
    9. Try the 'Podcasts' button and hover-over response in the dropdown menu for narrower screens. - Success
    10. Try the 'Trade Ideas' button and hover-over response in the dropdown menu for narrower screens. - Success
    11. Try the 'Contact Us' button and hover-over response in the dropdown menu for narrower screens. - Success
    12. Try the 'facebook' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    13. Try the 'twitter' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    14. Try the 'instagram' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    15. Try the 'Chat with Traders' link in the podcast title, and hover-over response in the podcasts section. - Success
    16. Try the 'The Investors Podcast' link in the podcast title, and hover-over response in the podcasts section. - Success
    17. Try the 'Macro Voices' link in the podcast title, and hover-over response in the podcasts section. - Success
    18. Try the 'Top Traders Unplugged' link in the podcast title, and hover-over response in the podcasts section. - Success
    19. Check the podcasts.html page in responsinator: <a href="https://www.responsinator.com/?url=https%3A%2F%2Fsammckenna1986.github.io%2Fmilestone_project_1-static_frontend%2Fpodcasts.html"></a>
    - iPhone eXpensive portrait · width: 375px - Success
    - iPhone eXpensive landscape · width: 734px - Success
    - Android (Pixel 2) portrait · width: 412px - Success
    - Android (Pixel 2) landscape · width: 684px - Success
    - iPhone 6-8 portrait · width: 375px - Success
    - iPhone 6-8 landscape · width: 667px - Success
    - iPhone 6-8 Plump portrait · width: 414px - Success
    - iPhone 6-8 Plump landscape · width: 736px - Success
    - iPad portrait · width: 768px - Success (ipad looks great)
    - iPad landscape · width: 1024px - Success (ipad looks great)
    
4. <b>User Story 4:</b> Looking for quick and easy trading ideas: tradeideas.html page.
    1. Try to read all of the text on the 'trade ideas' page, make sure that the information is correct, and make sure that the text looks strong. - Success
    2. The background image now loads faster as I replaced the jpg files with the converted png files. - Success
    3. Try the 'Your Own Money Investments' link in the logo  - Success
    4. Try the 'Reading' button and hover-over response in the navbar. - Success
    5. Try the 'Podcasts' button and hover-over response in the navbar. - Success
    6. Try the 'Trade Ideas' button and hover-over response in the navbar. - Success
    7. Try the 'Contact Us' button and hover-over response in the navbar. - Success
    8. Try the 'Reading' button and hover-over response in the dropdown menu for narrower screens. - Success
    9. Try the 'Podcasts' button and hover-over response in the dropdown menu for narrower screens. - Success
    10. Try the 'Trade Ideas' button and hover-over response in the dropdown menu for narrower screens. - Success
    11. Try the 'Contact Us' button and hover-over response in the dropdown menu for narrower screens. - Success
    12. Try the 'facebook' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    13. Try the 'twitter' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    14. Try the 'instagram' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    15. Try the 'yahoo finance' icon & link, and hover-over response in the social links at the top of the page. - Success
    16. Try the 'trading view' icon & link, and hover-over response in the social links at the top of the page. - Success
    17. Try the 'morningstar' icon & link, and hover-over response in the social links at the top of the page. - Success
    18. Try the 'tastytrade' icon & link in the social links at the top of the page. - Success
    19. Make sure all of the information in the 'trading view' chart is readable on wide screen and on narrow screens. - Success
    20. Make sure all of the information in the 'income statement' is readable on wide screen and on narrow screens. - Success
    21. Make sure all of the information in the 'liabilities section of the balance sheet' is readable on wide screen and on narrow screens. - Success
    22. Make sure all of the information in the 'cashflow sheet' is readable on wide screen and on narrow screens. - Success
    23. Check the tradeideas.html page in responsinator:<a href="https://www.responsinator.com/?url=https%3A%2F%2Fsammckenna1986.github.io%2Fmilestone_project_1-static_frontend%2Ftradeideas.html"></a> 
    - iPhone eXpensive portrait · width: 375px - Success
    - iPhone eXpensive landscape · width: 734px - Success
    - Android (Pixel 2) portrait · width: 412px - Success
    - Android (Pixel 2) landscape · width: 684px - Success
    - iPhone 6-8 portrait · width: 375px - Success
    - iPhone 6-8 landscape · width: 667px - Success
    - iPhone 6-8 Plump portrait · width: 414px - Success
    - iPhone 6-8 Plump landscape · width: 736px - Success
    - iPad portrait · width: 768px - Success 

5. <b>User Story 5:</b> User has a more specific question and wants to contact the website owner: contact_us.html page.
    1. Try to read all of the text on the 'contact us' page, make sure that the information is correct, and make sure that the text looks strong. - Success
    2. The background image now loads faster as I replaced the jpg files with the converted png files. - Success
    3. Try the 'Your Own Money Investments' link in the logo  - Success
    4. Try the 'Reading' button and hover-over response in the navbar. - Success
    5. Try the 'Podcasts' button and hover-over response in the navbar. - Success
    6. Try the 'Trade Ideas' button and hover-over response in the navbar. - Success
    7. Try the 'Contact Us' button and hover-over response in the navbar. - Success
    8. Try the 'Reading' button and hover-over response in the dropdown menu for narrower screens. - Success
    9. Try the 'Podcasts' button and hover-over response in the dropdown menu for narrower screens. - Success
    10. Try the 'Trade Ideas' button and hover-over response in the dropdown menu for narrower screens. - Success
    11. Try the 'Contact Us' button and hover-over response in the dropdown menu for narrower screens. - Success
    12. Try the 'facebook' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    13. Try the 'twitter' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    14. Try the 'instagram' icon & link, and hover-over response in the social links at the bottom of the page. - Success
    15. Try typing into the 'Email Address' field - Success
    16. Try picking all options: 'Particular Stock', 'Strategy', 'Position Sizing', 'Entering a Trade', 'Exiting a Trade' from the 'Question Subject' dropdown menu. - Success
    17. Try typing into the 'Question' field. - Success
    18. Try hovering over the 'Submit' button - Success (the full functinality of this form is out of scope for this static website project)
    19. Check the contact_us.html page in responsinator: <a href="https://www.responsinator.com/?url=https%3A%2F%2Fsammckenna1986.github.io%2Fmilestone_project_1-static_frontend%2Fcontact_us.html">Link</a>
    - iPhone eXpensive portrait · width: 375px - Success
    - iPhone eXpensive landscape · width: 734px - Success
    - Android (Pixel 2) portrait · width: 412px - Success
    - Android (Pixel 2) landscape · width: 684px - Success
    - iPhone 6-8 portrait · width: 375px - Success
    - iPhone 6-8 landscape · width: 667px - Success
    - iPhone 6-8 Plump portrait · width: 414px - Success
    - iPhone 6-8 Plump landscape · width: 736px - Success
    - iPad portrait · width: 768px - Success 
    - iPad landscape · width: 1024px - Success 


## Deployment

This section should describe the process you went through to deploy the project to a hosting platform (e.g. GitHub Pages or Heroku).

In particular, you should provide all details of the differences between the deployed version and the development version, if any, including:
- I deployed the website on github pages: <a href="https://sammckenna1986.github.io/milestone_project_1-static_frontend/index.html">Link</a>



## Credits
- Thank you to Antonio Rodriguez my mentor who's two meetings on this project were excellent and helped me understand a few concepts that I was missing.
- Thank you to Neil Kavanagh for clarifying a few concepts on the phone and for providing some extra motivation.
- Thank you to all the teachers on the course; The videos and excercises were excellent.

### Content and Media
- I wrote all of my own content.
- 'Balance sheet', 'cashflow sheet', and 'income statement' on the 'trade ideas' page were screenshotted from <a href="https://finance.yahoo.com/quote/WTI/balance-sheet?p=WTI">Yahoo Finance</a>
- The links and incon images for the books were taken from amazon.com
- The podcast icon images came from google images and from the podcast websites themselves.
- The pictures were copyright free and were downloaded from https://pixabay.com/.


### Acknowledgements

- I received inspiration for this project from my friends who are always asking me for suggestions on how they can start investing and trading. 

<b>I got a lot of information and inspiration for code from the following links:</b><br><br>
<a href="https://designshack.net/articles/trends/best-website-color-schemes/">https://designshack.net/articles/trends/best-website-color-schemes/</a>

<a href="https://www.pexels.com/photo/apple-devices-books-business-coffee-572056/">https://www.pexels.com/photo/apple-devices-books-business-coffee-572056/</a>

<a href="https://www.designwizard.com/blog/design-trends/colour-combination">https://www.designwizard.com/blog/design-trends/colour-combination</a>

<a href="https://tilda.cc/colors/">https://tilda.cc/colors/</a>

<a href="https://github.com/chartjs/Chart.js">https://github.com/chartjs/Chart.js</a>

<a href="https://stackoverflow.com/questions/45415678/is-this-possible-to-bookmark-a-page-with-html-button">https://stackoverflow.com/questions/45415678/is-this-possible-to-bookmark-a-page-with-html-button</a>

<a href="http://www.javascriptkit.com/dhtmltutors/cssmediaqueries2.shtml">http://www.javascriptkit.com/dhtmltutors/cssmediaqueries2.shtml</a>

<a href="http://stephen.io/mediaqueries/">http://stephen.io/mediaqueries/</a>

<a href="https://css-tricks.com/places-its-tempting-to-use-display-none-but-dont/">https://css-tricks.com/places-its-tempting-to-use-display-none-but-dont/</a>

<a href="https://stackoverflow.com/questions/40027058/bootstrap-remove-column-margin">https://stackoverflow.com/questions/40027058/bootstrap-remove-column-margin</a>

<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe">https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe</a>

<a href="https://codeburst.io/making-a-calculator-with-basic-html-css-and-javascript-part-1-1e4288f0bea1?gi=533a9abffa5f">https://codeburst.io/making-a-calculator-with-basic-html-css-and-javascript-part-1-1e4288f0bea1?gi=533a9abffa5f</a>
<a href="https://stackoverflow.com/questions/35816007/bootstrap-button-href-does-not-work">https://stackoverflow.com/questions/35816007/bootstrap-button-href-does-not-work</a>
<a href="https://www.w3schools.com/howto/howto_css_image_center.asp">https://www.w3schools.com/howto/howto_css_image_center.asp</a>


