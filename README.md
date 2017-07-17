## Welcome!

This is an introduction to the learning approach and resources that we have developed in the group. The overall goal is to learn how to use the R statistical computing language for day-to-day business tasks by investigating interesting non-financial datasets. For most of us, R can be a useful extra tool to use alongside Excel, Tableau and our other analysis applications.

## Why Now? 
Excel will remain a central analysis tool for all of us. However these are some of the things that you might do more easily with R than with Excel a little practice:-

* create a reliable, readable, documented record of a data analysis process. No reliance on opaque spreadsheet formulas, pivot table setups, recalculation and fragile VBA code which make teamwork and checking difficult
* easily create top-quality, modern, legible charts with much more control than Excel

## The context

* We now have more data available that we would like to analyse. Excel hasn’t risen to the challenge. Although it's nice to have a full dataset available to view and edit, and although spreadsheet formulas are familiar and intuitive, they do not scale up well.
* The open-source software movement, notably R, has recently created many powerful and easy-to-use tools that are directly relevant to our work.
* When we don’t have up-to-date skills, we fall behind current best practice. (This is bad for our business, and our careers.)
* In general, our 'subject matter expertise' is hard to learn and reproduce, but learning data analysis skills is quite straightforward. So it makes sense for us to learn the latter, in order to further improve our mastery of the former.

## Why is R a good choice?

* It's free.
* It has a long track record.
* There's lots of help and tutorials online that usually quickly solve almost any problem that you will encounter. (Even more more help than you will find online for Excel, for example.)
* Most R users are researchers and business analysts, not programmers. This maybe explains why the online communities around R are quite user-friendly for non-programmers.
* Traditionally, R was quite hard to approach. For many years there were several good tools available for each task, but no guidance on which would give the best immediate or long-term results for developing a project. Happily, over the past 5 to 10 years, a collection of R packages, sometimes called the 'Tidyverse', has been developed which offers a comprehensive and consistent set of tools for most basic business data manipulation and visualisation tasks.
* There are thousands of specialised packages that we can install in R which handle more unusual analysis problems, including all the latest statistical and machine learning techniques. All are free.

## What can I do in R that I can't do in Excel?

If you haven't used R before, and after spending a short time learning, the following should be quite easy for you:-

* create legible, attractive, modern charts
* clear, transparent formulas for calculations
* easy, robust recalculations of very large datasets
* (at work) improved productivity in creating and updating your analyses

After learning a bit more, you'll probably be able to do the following (and more) better than you can in Excel:-

* codified end-to-end processes (import, clean, transform, summarise, model, chart, export...)
* audit trail
* teamwork
* source control, version comparison
* text analysis
* machine learning

## Getting set up: basic requirements

1. A computer with internet connection and Chrome or Firefox browser. Note you can't develop Kaggle kernels with Internet Explorer.
2. Kaggle account. Get a username: https://www.kaggle.com

## What are Kaggle kernels? 

Kaggle is a website that organises data science competitions. One of the company's key goals is education and building data analysis communities, and there is no need to take an active part in competitions to benefit from its resources. In particular, we can make use of (i) a wide range of interesting datasets that Kaggle has curated and made available for use; and (ii) a cloud-based computing environment which allows us to analyse these data using R, Python and other open-source data analysis computing languages. This is very convenient because the virtual computers that Kaggle lets us use are very similar to what we would set up if we would install these languages on our own desktop PCs, but without the hassle of installing the software. Kaggle supports a number of open-source data analysis software environments, including Python and R. We have chosen R as we have found that it is a nice language for getting started, though more experienced group members use a variety of other languages too. When we create a Kaggle 'kernel' we are using Kaggle's computing environment, together with one of the datasets, free of charge, to develop code and documentation to analyse the data. By having a Kaggle user account, we get access to these resources, and our work is stored so that we can continue developing it at a later date, or sharing it with others, in any location with an internet connection.

## Playing with the Kaggle kernels

In our first sessions, we looked at a few kernels where we tried to illustrate some basics of data analysis in R. Here are steps for getting started with running the code and editing it yourself:-

1. Log in to Kaggle
2. Search for user 'axaimdc' in the Kaggle search box
3. Click on the kernel that you want to work on
4. You'll now see the full 'notebook' view of the kernel, probably including a mixture of narrative text, pictures, R code cells (labelled `In []`) and output from the R session (labelled `Out []`)
5. Click on the blue button 'Fork'. This will (i) create your own copy of the kernel; and (ii) launch a virtual computer session which you can use for running the code in the kernel.
6. You can click on one of the 'cells' in the kernel, and run the code by pressing the 'execute' button that appears (or by pressing Shift+Enter). You should see the computer running the command for a short time, then returning the output and/or error messages.
7. Move down to the next cell that you want to run. You can edit the code if you like, then run that cell. 
8. There are also buttons that let you add a new cell above or below the one that you're working on, or delete the cell. 
9. Your work will be saved automatically, and you can resume work later by following the instructions below.

## What happens during the R session?
The R code might initially look confusing. In general, this is what is happening as we continue our analysis: 

* Firstly, we have to import some data into the R session. This usually means getting R to open a CSV file (or spreadhseet) and putting the table of data in that sheet into a **dataframe**. 
* We give the dataframe which contains our data a name, often `df`.
* Just like well-organised a spreadsheet, the dataframe has named **columns**, and a certain number of **rows** of data. That’s why we can easily apply spreadsheet-like actions to it like sorting or filtering.
* After doing some analysis, we might put part of the dataframe into a new dataframe, perhaps with a different name. At this point, both dataframes are available for further analysis. 
* At each subsequent step, we are generally taking one of our existing dataframes and doing some kind of transformations on the data, either to produce more data, to produce a chart, or to export the data for use elsewhere, perhaps in a spreadsheet.

## A couple of quirks in R
Here's a couple of things that might seem odd at first in R for those who are more familiar with Excel, VBA or any traditional programming language. Don't worry if this seems unclear, by looking at a few examples you will soon get the hang of it.

**`<-`** this is the *assignment* operator. It is supposed to look like a backwards arrow (see?) For example, when we execute 
`b <- 2`, we are assigning the value of `2` to `b`. This seems odd at first: in most programming languages, you would assign with 
`b = 2`.

**`%>%`** this is the *pipe* operator. See examples in the kernel notebooks for how this works. It is part of an R package called magrittr.


## If the session becomes unresponsive
Kaggle kernels are not as reliable as having R installed on your local PC. Sometimes the kernel session seems to become unresponsive. It may help to press the 'Restart' button at the top, or to reload the whole page in your browser. In either case, you'll start a new computer session so you'll have to re-run the steps that you took in your previous session to get your data back to its previous state. 

## Resuming work on a kernel that you previously created/forked:-
1. Log in to Kaggle
2. Click on Kernels, then select filter to see your personal kernels by clicking on 'Mine' . You can then choose the kernels that you already have, including those that you previously forked (and edited) from the axaimdc account.
3. Click on the blue 'Edit Notebook' button. (You may have to agree to 'competition rules' if you're using one of the 'competition' datasets.) This will launch a virtual computer that you can use for editing and running your R code.
4. You'll need to re-run the code cells that you previously wrote if you want to see/refresh the output tables and charts.

## More tips for working in Kaggle kernels

* Your kernel (the one that you forked from the original kernel) is private, and cannot be seen by other users, until you click on `Public` at the top of the kernel. After this, you can share the URL for your kernel with others who will see it.
* If you want to make your work *really* public, click on `Publish`. Then  your work will appear in the list of the latest work under way on the particular Kaggle dataset that you're looking at. In this case, please be aware of the usual privacy issues...
* Your work is regularly saved automatically. However the latest version is only available for others to see after you have (i) made the kernel Public (see above) and (ii) exited from the kernel session.


## Moving from Kaggle kernels to RStudio

In later sessions we might do some analysis in RStudio instead of Kaggle kernels. This is a nice tool which works well for day-to-day desktop analysis jobs.

1. Install R. Google ‘download r’. Choose a nearby ‘CRAN mirror’ location, and click on a download link. Takes a minute or two to download.
2. Install RStudio (search ‘download Rstudio’). Download the ‘free’ version. This is the desktop GUI which makes it easier to use R.
3. Try launching RStudio. If  you see a ‘console’ window with some copyright notices and a flashing cursor, then you are ready to continue.
4. Start installing the packages that you need, for example:
install.packages('tidyverse')
5. I’ll create ‘.r’ files based on the Kaggle kernels which we can use as an alternative to the Kaggle kernels.


## References: Favourite Data Sources

https://public.enigma.com/

https://data.gov.uk/

https://data.london.gov.uk/dataset
