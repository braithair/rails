# rails
A Rails code repository

2018-07-02

--Contents--

1. Platform
-- Amazon EC2 Instance 

2.  Ruby
-- Installing Ruby

3.  Rails
-- Installing Rails


--Details --
1. Platform
It was decided that an EC2 instance on AWS would be suitable to begin with at it is free.
The instance under Utilisation is operated by 'braithair'.

  a. Installing
  Setting up an Amazon instance is quite simple, it consists of:
    i.    Setting up an Amazon Account
    ii.   Starting your EC2 instance
    iii.  Downloading your SSH key (to remotely access)
    iv.   Testing your Amazon instance for connectivity.

2. Ruby
Ruby is a fundamental piece of the puzzle to understand Rails. It is needed for the comprehension of and implementation of Rails.

  a. Installing
  A great guide to installing Ruby on an Amazon Linux system is here:       https://www.phusionpassenger.com/library/walkthroughs/deploy/ruby/aws/nginx/oss/install_language_runtime.html
  This installer goes through the setup of:
    i.    Preparing the system
    ii.   Installing RVM (Ruby Version Manager)
    iii.  Installing Ruby version of choice
    iv.   Installing Bundler (for gem dependencies)
    v.    Installing node.js (optional)

3. Rails
Once you have Ruby, you can install Rails knowing you have some necessary pieces of the puzzle.

  a. Installing
  A great guide to install Rails on a Linux system is here:
  http://guides.rubyonrails.org/getting_started.html
  This installer goes through the setup of:
    i.    Checking Ruby version
    ii.   Installing SQLite3
    iii.  Installing Rails
    iv.   Creating the 'Blog' tutorial application
    v.    Starting the web server.
    vi.   Setup and using rails (multiple steps from sections 4.2 to 9)
    vii.  Setup and using Rails. I installed rails blog from 4.2 in /src
  All the important stuff happens in sections 4.1 through to 9.
 
  b. Starting the web Server
  When starting the webserver on Rails, using Amazon EC2, you need a few things first.
      1. Bind your rails server to the local IP of your Amazon EC2 instance
      I used: $   bin/rails server -p 3000 -b 172.x.y.z (x.y.z is your instance IP)
  
  Then, make sure you add a "Security Group" in the Amazon instance and open the port to your accessing PCs public IP. This will allow you to get onto the Rails server you started above. You will know when it works because it will show the splash page in your broswer when you use the Public IP and port you whiteliste for your Amazin instance. It will say "Yay! you're on Rails!". This is notated by section 4.1 in http://guides.rubyonrails.org/getting_started.html. Use "Ctrl + C" when you are ready to stop the Rails server for now.
  
  c. Getting Rails to say "Hello"
  Run: $   bin/rails generate controller Welcome index.
  
  The above will make file and routes for you. So next path to your newly created folder which will be where you installed the Blog as part of sectiont 3aiv above. Mine was in /src/blog/app/views/velcome . From there vim the "index.html.erb" file and add a h1 heading html tag and the text: "How bouh dah". Then close the tag and write the file.
  
  d. Setting the home page
 Go to: the 'config' directory in your blog folder. mine was in /src/blog/config. Use VIM to edit the "routes.rb" file. Add into the 'routes.rb' file: root 'welcome#index'. Then save the file
 
  
  
 
 
 
