# napari plugin installation workflow
Sometimes you may need to perform a task that isn’t currently done in napari. napari can be extended using plugins written by the napari community. This is a fairly detailed flowchart of the steps needed to install a plugin into napari. [Written steps summarizing the flowchart](#written-steps-summarizing-the-flowchart) follow.  

![plugin installation workflow](.\images\plugin-installation-workflow.png)  

## Written steps summarizing the flowchart  

- Search [napari-hub.org](napari-hub.org) for a plugin.  
  - Is there an appropriate plugin?  
    - Make note of plugin data:  
      - name  
      - prerequisites  
      - any other details needed  
    - Make sure all prerequistes are met.  
- Open napari  
  - Go to **File**>**Plugins**>**Install/Uninstall plugins**   
  - Search for the plugin in the list of available plugins.  Enter the name or partial name of the plugin in the filter box to narrow the search.  
    - Is the plugin available?  
      - Click install button on right end and wait for installation to complete.  
      - Verify the plugin shows as installled in the list of installed plugins.  
      - If the pluging appears in napari Plugin list, launch it and use it.  
   - If, after installing the plugin from the list of available plugins, it does not appear in the list of installed plugins:  
    - Close and reopen napari.  
      - If the pluging appears in the list of installed plugins, launch it and use it.  
      - If not, refer to plugin documentation on napari-hub.org for  instructions, i.e. Some form of manual installation, such as using pip install on the command line: `python -m pip install plugin-name`.  

- If the plugin still does not appear in the napari plugin list, seek help from the plugin developer. 

If there is not an appropriate plugin, find another solution, such as:  
- Ask on Zulip for plugins not available on napari-hub.  
- Ask fellow researchers if they are aware of other plugins that solve the problem or how they found other potential plugins that may help.  
- Write a plugin of your own.  