# _{WikiCat}_

#### _{It is an API based application that has WikiPedia categories and related links. It is not designed to be a stand alone application. It's partners will be mentioned here when they are available.}, {4/9/2016}_

#### By Chris Underwood

## Description

_{It is an API based application that has WikiPedia categories and related links. The API is version 1 and can be found under app/controllers/api/v1. There are 4 main paths to get data from the API: 1) http://localhost:3000/api/v1/graph/ which brings up the Main Topic Classifications, 2) http://localhost:3000/api/v1/graph/(category such as arts) which will bring up the subcategories under that category, 3) http://localhost:3000/api/v1/graph/up/(category such as arts) is to be used by another app in ways that I have not fully flushed out, 4) http://localhost:3000/api/v1/category/(category such as arts) shows the info about that category such as number of subcategories and urls to find other data in the system about the category.}_

## Setup/Installation Requirements

To install ruby, rails, and mysql, here is a good start: https://gorails.com/setup/osx/10.10-yosemite

To user the seed files, rename the not-seeds.rb file in db and run rake db:setup from the normal mac command line once you have mysql installed and running.

If you want to use the full files you will need to use the mysql command line to run sql commands via folder. Using the mysql command line, you will need to be in the proper database. Then run the script via the mysql command line. https://dev.mysql.com/doc/refman/5.7/en/mysql-batch-commands.html

To get to the mysql command line follow this link: http://stackoverflow.com/questions/22391778/mysql-command-line-bash-command-not-found

If the program is stopped and you want to start it again, say if the computer was turned off, you go to the commmand line and migrate the folder that contains the application. Type in mysqld & <return> and then type in another tab of the command line rails s <return>.

_{Leave nothing to chance! You want it to be easy for potential users, employers and collaborators to run your app. Do I need to run a server? How should I set up my databases? Is there other code this app depends on?}_

## Known Bugs

Not sure if the up function in the graph controller is working properly.

Not so much a bug as a warning. Loading the full SQL files can take many hours. The links file took my MacBook over 12 hours. I suggest loading the seeds file first to make sure you want to go through the effort to load all of the data.

## Support and contact details

_{Feel free to contact me at cunderwoodmn @ gmail dot com.}_

## Technologies Used

mysql 5.7.11
rails 4.2.5
ruby 2.2.2
gems
  responders
  rails-api
  active_model_serializers

### License

Please note that much of this code is from the RESTFull Rails Development book from Silvia Puglisi. You should be sure to contact the author is you want to use any of this code in a production (i.e. money making environment).

Copyright (c) <2016> <Chris Underwood>


Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
