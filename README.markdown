# SBT Plugin examples 

---
    
This was prepared for a talk on developing SBT Plugin I gave at PHASE meeting one 
time in january 2012. The presentation is [here](https://raw.github.com/mads379/sbt-plugin-examples/master/Building-SBT-Plugins.pdf "here").

---

The following project contains three plugins 

- A plugin that provides a command
- A plugin that provides some settings 
- a plugin that provides a command with tab completion!

The `playground` project shows a convenient way to depend on your
plugin locally so you get a fast turn-around in development when 
you just want to try out the plugin without having to publish it etc. 
you simply just make the changes to want to your plugin and then run `reload`
in the playground project. 

`cd` into the playground project and start an SBT shell: 
    
    # run the command from the command plugin
    > hello 
    # run the task in the settings plugin 
    > new-task
    # have some fun with the setting and run it again
    > set newSetting := "Hi PHASE!!!"
    > new-task
    # play with the tab-completion (try pressing tab all the time)
    > ask-phase brian would you like to buy mads a beer?
 