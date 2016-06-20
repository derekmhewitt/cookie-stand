# cookie-stand

## Problem domain:

Pat's Salmon Cookies
- needs to calculate the number of cookies each location must make every day so that it can manage its supplies inventory and baking schedule.
- The number of cookies to make depends on the hours of operation (6:00 AM to 8:00 PM for all locations) and a few factors unique to each location:

1. The minimum number of customers per hour.
2. The maximum number of customers per hour.
3. The average number of cookies purchased per customer.
4. Because we are early in the life of this business, we will need to build an application that is adaptable.
5. Pat will need to be able to add and remove locations from the daily projections report, and
6. Pat will also need to be able to easily modify the input numbers for each location based on day of the week, special events, and other factors.
7. Pat would like to see these numbers with nice formatting in a web application
8. Pat needs you to take a leading role in doing the design work and construction of a public-facing page, too. Pat has a logo image picked out, but that's it.
9. Pat has asked you to come up with all other aspects of the design for both documents, including
- a color scheme and a custom font, and maybe additional images, for a public-facing webpage.

Build an application that
- calculates daily sales projections for each location (in a file called sales.html),
- create a pubic-facing page (in a file called index.html) that is colorful, eye-catching, readable, useful, informative... and ultimately of a quality ready for use on T-shirts, stickers, coffee mugs, cookie bags, napkins, and so on.


Calculate Daily Sales Projections (sales.html)

We're going to assemble this web application bit by bit.

First, create a separate JS object literal (no constructor functions... yet) for each shop location that does the following:

Stores the min/max hourly customers, and the average cookies per customer, in object properties
Uses a method of that object to generate a random number of customers per hour. Objects/Math/random
Calculate and store the simulated amounts of cookies purchased for each hour at each location using average cookies purchased and the random number of customers generated
Store the results for each location in a separate array... perhaps as a property of the object representing that location
Display the values of each array as unordered lists in the browser
Calculating the sum of these hourly totals; your output for each location should look like this:

1st and Pike

6am: 16 cookies
7am: 20 cookies
8am: 35 cookies
9am: 48 cookies
10am: 56 cookies
11am: 77 cookies
12pm: 93 cookies
1pm: 144 cookies
2pm: 119 cookies
3pm: 84 cookies
4pm: 61 cookies
5pm: 23 cookies
6pm: 42 cookies
7pm: 57 cookies
8pm: 29 cookies
Total: 657 cookies
Display the lists on sales.html. We will be adding features to this application and working with its layout throughout the week.

Here are the starting numbers that you'll need to build these objects:

Location	Min / Cust	Max / Cust	Avg Cookie / Sale
1st and Pike	23	65	6.3
SeaTac Airport	3	24	1.2
Seattle Center	11	38	3.7
Capitol Hill	20	38	2.3
Alki	2	16	4.6
These numbers are simply Pat's estimates for now, but eventually, once there has been some history collected that provides more accurate numbers, we'll want the ability to update these numbers for each location, and to add/remove locations. But we'll not build all of that today. Make sure to make each location is its own JavaScript object.

Public-Facing Page (index.html)

Besides using the picture of the fish... you should use...

A custom Google font for highlights
A specified standard san-serif web font for data (such as Arial, Verdana, or Helvetica)
A specified standard serif web font for text (such as Georgia, Times, etc.)
Specified different font colors for all three font usages
A background color for the default page background (make sure font colors have good contrast and are readable on this background)
A different background color for elements such boxes and tables (so make sure the font colors contrast against this well, too!)
Anything else you'd like to add related to style. But remember: simplicity, clarity, and consistency are good things in design.
Be thoughtful about layout and overall organization of the page.
Include all of the typical stuff that you'll find on the home page of a business: locations, hours, contact information, some text about how awesome the business is, etc. Be creative, and again, think about what is meaningful to a typical end user.
