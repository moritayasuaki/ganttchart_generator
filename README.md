# Gantt Chart Generator
This is an add-on for Google apps script. You can automatically create a gantt chart, which is suitable to manage a small or middle project. English & Japanese are available.



![f:id:takuya0206:20171223222331g:plain](https://cdn-ak.f.st-hatena.com/images/fotolife/t/takuya0206/20171223/20171223222331.gif)


## Installation

[Gantt Chart Generator - Google Sheets add-on](https://chrome.google.com/webstore/detail/gantt-chart-generator/bnaicalmdphddkedcgchnfbjohmhdgni?utm_source=permalink)

Access the above URL, log in your Google account, and click "＋ Free."


## What You Can Do

* Break down tasks into five levels
* Automatically paint a chart based on a date you enter
* Automatically calculate workloads related to a parent task
* Automatically place bars based on progress you enter
* Automatically calculate progress related to a parent task based on workload weight
* Edit holidays as you want (*the default is Japanese holidays)


## Specification

### Add-on Menu

Item         | Action                     
---------- | -------------------------
Create Gantt Chart | Create a schedule sheet and a holiday sheet
Show Sidebar   | Show a sidebar                 

### scheudle sheet

Item           | Input  | Action                                    
------------ | --- | ----------------------------------------
Work Breakdown Structure    | String | Assign task ID                                   
Planned Start & Planned Finish | Date  | Paint a chart in blue                           
Planned Finish         | Date  | Set a milestone in orange                        
Actual Start & Actual Finish | Date  | Paint a chart in green（*be hidden in the default）                
Worklaod(plan)        | Number  | Calculate parent's workload                               
Progress           | Number  | Place bars in a chart & calculate parent's progress if tasks have workload (plan)  


### holiday sheet

Item | Input | Actuon               
-- | -- | -------------------
A column | Date | Make a holiday line in pink

### Sidebar

Item           | Action                      
------------ | --------------------------
Change Start Date       | Cange start date in a gantt chart          
Recalculate Workload (plan) & Progress | Calculate all parents' worklaod and progress             
Repaint Gantt Chart | Repaint all of the Chart         
Show Color Indication      | Indicate progress like blue means "completed," yellow means "in progress" and red means "delayed"
Show Parents' Charts      | Automatically show total duration of parents' charts
Initalize Gantt Chart          | Initalize schedule sheet and holiday sheet

## Recommended Usage

* Place a project name in the top hierarchy and make all of the tasks its children. That is to say, you can automatically calculate progress of your project.
* Break down tasks in detail like Parent tasks, child tasks and grandchild tasks.
* Place planned start and planned finish in tasks which you have to watch daily or weekly.
* Use "show parents' charts" when you check progress from a broad viewpoint.
* Utilize "workday function." You can refer to A column in holiday sheet and workload (plan).
* Place workload in man-day.
* Watch progress by using actual start and actual finish or progress bars.
* If you use progress bars, you may want to active "Color Indication."
* If you update numbers in progress column by using functions, charts won't be automatically updated. You need to use "Repaint Gantt Chart."

## Restriction

* Do not change the sheet name (schedule sheet and holiday sheet).
* Do not insert rows before the item row.
* Do not edit or delete the hidden second row.
* Do not insert columns between the start and the finish date column and after the progress column.

## License
GNU General Public License (GPL)

## FAQ

 - How do I extend the width of my gantt chart?

The width of a gantt chart can not be changed and is fixed for 168 columns, which means 24 weeks. If you'd like to show after the period, you can do it by using "Change Start Date" in the sidebar.

 - How do I change the color of charts?

The color of charts can not be changed as you like. In the current specification,  Show Color Indication is the function related to change of color.

## Privacy Policy
We treat your privacy with respect and it is secured and will never be sold, shared or rented to third parties.

### Information We Collect
In operating our add-on, we may collect and process the following data about you:

* Details of your visits to our website and the resources that you access, including, but not limited to, traffic data, location data, weblogs and other communication data
* Information that you provide by filling in forms on our website, such as when you registered for information or make a purchase
* Information provided to us when you communicate with us for any reason.

