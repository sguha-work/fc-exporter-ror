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


### Usage Guide
* After installing the plugin you have to activate the plugin by moving on to the plugins page of wp-admin and clicking on activate of "Fusioncharts For Wordpress" plugin
* After activating it you will found "Create fusionchart for this Page/Post" button on every edit post/page page of Wordpress admin panel like screenshot 1
* Clicking on the button will open a Fusionchart settings form like screenshot 2, You have to fill up the form with desired values. All form element contains default values, Event there is sample JSON data which can be used to populate basic charts for more example on FusionCharts visit "http://www.fusioncharts.com/charts/"
* After the form is filled up you may preview the chart as shown in screenshot 3. If any more changes needed you may go back to settings page or you may go to next step to embed the chart.
	* If there is any error in chart data the chart will not be populated
* In the last step you will found a text area having raw html and JavaScript code like screenshot 4, you have to copy the entire code and then go to text mode editor of the page & post and paste the code where you like to see Fusionchart.
* Update the page/post and see interactive JavaScript charts in your page/post

### Screenshots
1. Here is the button on the top right side of the edit page of a Wordpress page to start
	![Screenshot1](http://i.imgur.com/GRCGemK.png)
	
2. Here is how the chart settings form looks like
	![Screenshot2](http://i.imgur.com/oaP7lp5.png)
	
3. Here is the preview of the chart
	![Screenshot3](http://i.imgur.com/Jm2eJwY.png)		
	
4. Here is the embed chart section along with the code
	![Screenshot4](http://i.imgur.com/lvAYx98.png)
	
5. Here is the sample page with Fusionchart
	![Screenshot5](http://i.imgur.com/oB8rDdo.png)

### Frequently Asked Questions ==
* What about FusionChart?
	* Well you may just put the query in Google. :) Please visit http://www.fusioncharts.com/ to know the awesome
* Can I use a paid version of FusionChart with this product
	* Well obviously you can, you just have to unzip all the files you got from purchased product inside "wp-content/plugins/fc-wp/assets/fc-assets/" folder replacing the existing files

### Upcoming features
1. Chart type specific example data both XML and JSON
2. Improvement in the UI

### Change-log
== v0.23 ==

1. Fusioncharts libraries updated to latest version 3.10
2. Two new chart types added Treemap chart and Zoom Scatter chart


== v0.22 ==

1. Bug fix in parsing XML data
2. Bug fix in parsing JSON data
3. Chart type specific example data both XML and JSON
== v0.21 ==

1. Bug fix in chart generation library
2. Changed sample data population
3. UI changes
 
== v0.2 ==

1. Added the feature to have data from JSON/XML url.

### If any issue found or wish to request improvements feel free to drop a mail at sguha1988.life@gmail.com
