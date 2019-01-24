# Async-Inn

Ryna Truong
Deziree Teague
Shalom Belaineh
 
Relational Database

We created a branch with a primary key BranchID#, name, number of rooms, and a composite key relationship to room type that is room ID# and location ID#. This branch has navigation properties that navigate to site, guest, and room type. It has a many to many relationship with room type, and a one to one relationship with site.Within the room type we have a primary key, RoomTypeID#, layout, pet friendly, price, and a foreign key to amenities with navigation to branch and amenities. It has a many to many relationship to the amenities and branch. Amenities is our Enum, that navigates to room type, because room type will have specific amenities. These two have a many to many relationship. We have a site with a primary SiteID#, address, city, state, phone number and a foreign key of BranchID# that navigates to the branch. This site has a one to one relationship with branch. Guests will include a primary reservation ID#, including name, foreign key of room type, and a check in and check out.  They have a one to one relationship with both check in and check out, and a many to many relationship to bracnh. This navigates to Branch, and CheckIn, CheckOut which is our payload. It navigates to CheckIn, CheckOut, and also navigating to branch. For the check in and check out they both have the date, time, and foreign key reservation that navigates to guest. They both have a one to one relationship with Guest.

![Diagram](https://github.com/rynnnaa/Async-Inn/blob/master/AsyncInnNav.jpg)
