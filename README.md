# xy_plot_js
An R program that writes an interactive scatter plot in html5/canvas/javascript format

This project consists of an R program <code>xyplot_js.R</code> that writes a simple scatter plot (similar to the R function <code>plot</code>) in html format. The plot it writes is interactive: if the user moves the mouse over a point, the point changes color and a small popup label appears indicating its index and coordinates. (The idea is to allow the user to examine outliers or other interesting points.)

The project includes the R program itself, and four supporting files: The bulk of the output file cut into three "template" parts (e.g. <code>plot_template_part1.html</code>, and a stylesheet <code>styles.css</code>. The R program is designed to read the three template parts of the html file, and to write the specific material (data etc) for the plot to be written in between the template parts. This is designed to keep the R program as simple as possible (most of the output html is "pre-written" in the template files).

Everything is intended to be simple and hopefully easy to understand, so any interested programmer who knows R and some javascript may be able to tinker with the code (change formatting or add functionality). The overarching philosophy of this project is to make it easier to communicate mathematics visually, with self-contained code that is easy to understand and modify. (No specialized libraries are called. Such libraries might enable more interesting output that is more glossy, but then the user is at the mercy of resources that might change, become broken, or become unavailable. Also, use of external libraries or resources would get in the way of simplicity and also cost flexibility--the user would have less control over fine details or be stuck with default formats or styles.)

This repository includes a file, <code>faithful.html</code> that shows what typical output for this program looks like. It was written by the R program. 
