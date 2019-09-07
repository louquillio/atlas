# Atlas, a theme for Discourse

Atlas features an alternate topic list layout intended to highlight topic excerpts, and also includes space for an (optional) sidebar. Categories feature user-dismissable headers populated by the "About" topic. 

![12%20PM|625x499](https://d11a6trkgmumsb.cloudfront.net/optimized/3X/b/8/b8f1197639f15c182e9c2945e958ede81483639e_2_1250x998.png) 

:telescope: [Preview on theme creator]( https://theme-creator.discourse.org/theme/awesomerobot/atlas-theme) (note that excerpts aren't turned on, so the preview is a bit limited) 


:question:  https://meta.discourse.org/t/how-do-i-install-a-theme-or-theme-component/63682




:information_source: Important notes:

* The sidebars are added using the [Custom Sidebar component](https://github.com/awesomerobot/discourse-custom-sidebar) , which can be setup to feature a post as the sidebar content for specified categories. Configuration details are in the repo's readme. 

* The theme works best with the box category style (admin > settings)

* Excerpts can be enabled using a hidden site setting called `always_include_topic_excerpts`. To enable this setting you need console access to your server. 


  To enable excerpts via the command line

  ```
  ./launcher enter app
  rails c
  ```

  and then in the rails console

  ```
  SiteSetting.always_include_topic_excerpts = true
  ```






:hammer_and_wrench: Future improvements

* There are some hard-coded colors in this theme, I need to update those to be editable by color schemes

* Settings to turn certain features (like category headers) on and off
