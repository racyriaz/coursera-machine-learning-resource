# OCTAVE TOOLS FOR PLOTTING AND VISUALIZING DATA

+ plot(x, y, color,  )
+ `plot(x,y)`
+ use `hold on` to plot chart1 on new chart2
+ `xlabel('x axis name')`
+ `ylabel('y axis name)`
+ `legend('chart_1','chart_2')` &rarr; similar to chart keys
+ `title('my title')`
+ save the plot &rarr; `print -dpng 'myCharName.png'`
+ `figure(1); plot(x,y)` &rarr; gives plots a figure number
+ **subplots**
  + `subplot(1,2,1); plot(x,y)`
  + `subplot(1,2,2); plot(a,b)`
+ setting X and Y range / AXIS
  + `axis([0.5 1 -1 1])` &rarr; 0.5 to 1 is for X axis and -1 to 1 is for Y axis
+ clf &rarr; clear the figure screen
+ Visualize matrix with `imagesc(A), colorbar, colormap gray;` &rarr; gives a kind of heat-map with scale
