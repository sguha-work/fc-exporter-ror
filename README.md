# fc-exporter-ror
FusionCharts export handler in RubyOnRails

* Author: Sahasrangshu Guha
* Author URI: https://github.com/sguha-work/
* Requires at least: ruby 1.9.3p484 (2013-11-22 revision 43786) [i686-linux], Rails 4.2.5
* Tested up to: ruby 1.9.3p484 (2013-11-22 revision 43786) [i686-linux], Rails 4.2.5
* Stable tag: 0.1
* Version: 0.1 

This program is a controller of RubyOnRails which will export FusionCharts as JPEG, PNG, PDF, and SVG. Following are the installation guide and usage guide of the program.

### Installing
  Providing the links of guide to install ruby and RubyOnRails on system first
  
  See this official guide to install ruby [How to install ruby](https://www.ruby-lang.org/en/documentation/installation/)    
  And here is the link to [Getting Started with RubyOnRails](http://guides.rubyonrails.org/getting_started.html)
  
  Now if your RubyOnRails project is up and ready to be executable you have to do the following steps
  
1.	Copy the "fc_exporter_controller.rb" to the <root>/app/controllers directory
2.	Open the <root>/config/routes.rb file in text editor and add this line "post 'fc_exporter/init'" where the routes are defined
  There are 2 dependencies of the program, you have to install those gem also
1. rmagick: For this don't use "gem install rmagick" use the following steps
	First, check that the universe repository is enabled by inspecting '/etc/apt/sources.list' with your favourite editor.
 You will need to use sudo to ensure that you have permissions to edit the file.

 If universe is not included then modify the file so that it does.

 deb http://us.archive.ubuntu.com/ubuntu precise main universe
 After any changes you should run this command to update your system.

 sudo apt-get update
 You can now install the package like this.

 Install librmagick-ruby
 sudo apt-get install librmagick-ruby	
 
2. json: just use "gem install json" 


### Usage Guide

From a view where the FusionCharts is being displayed you can add the attribute "exportHandler" and the value "http://localhost:<PORT-NUMBER(eg. 3000)>/fc_exporter/init/" to use the export handler

### If any issue found or wish to request improvements feel free to drop a mail at sguha1988.life@gmail.com
