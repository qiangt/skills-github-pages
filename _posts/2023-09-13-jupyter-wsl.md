I am running Ubuntu 22.04 WSL under Windows 11. And I am using VS Code to do run some awesome pytorch3D scripts. However, it took me quite a while to figure out how to display the 3D graph properly with interaction. 

1. **Using VSCode and install the Jupyter addon by Microsoft:**
    - This allows you to change your python script to Jupyter notebook very quick. Just add "$ %%" on the top of the section where you want to run it as jupyter notebook
2. **The magic of "%matplotlib notebook"**
    - This is normally used to set the backend of the matplotlib. Therefore, you should add this line before anything other matplotlib imports to be safe.  
    - If you don't specify notebook backend, the default is inline. What's the difference? Notebook gives you interaction, which means you can interact with the figure, e.g., save, pan, zoom-in, etc.
    - BTW, this hasn't work for me yet. 
3. **How to display 3D figure properly**
    - People use mpl_toolkits, i.e., from mpl_toolkits.mplot3d import Axes3D
    - Below is the magic how to make it work. A lot of tutorial uses "ax = Axes3D(fig)" and it didn't work for me.
    > ax = fig.add_axes(Axes3D(fig))
    > 
    > ax.scatter3D(x, z, -y)    
