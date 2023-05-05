Add this in the layout.html footer

                <div class="pull-right">
                    {{ 
                        if auth.user != None: 
                            #if 'admin' in auth.user_groups.values(): 
                                =LOAD('plugin_log', 'index.load', ajax=True) 
                            #pass 
                        pass 
                    }}
                </div>

And check controllers/plugin_log for routes that can be added to the menu