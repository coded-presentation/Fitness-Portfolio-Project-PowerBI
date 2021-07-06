
<div class="site-branding">
	<h1 >:watch:Fitbit Data Analysis</h1>
<p class="site-description">This Data Analyst Portfolio-1, This Example is only for getting started with cleaning, Organizing, Exploration and Visualization in Power-BI </p>
</ul></div>				
 
<h4 class="entry-title">Data Analyst Portfolio Project-1 – Fundamentals of Excel & Power-BI</h4>	
		
			

<div ><table><tr><td><img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data.png?w=400"></td><td><img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2.png?w=565?w=400g"></tr>
	<figure class="coblocks-gallery--figure">
	<td><img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model.png?w=411g"></td>
	<td><img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/power-bi-applied-steps.png?w=524g"></td></tr></table></div>

<hr class="wp-block-separator is-style-wide">

<h2>:milky_way: Business Request &amp; User Stories </h2>



<p>The business request for this project was created by karan shah. By deciding on a business processes to analyze (exercise data) the following user story was derived.</p>

<table><tbody><tr><td><strong> #</strong></td><td><strong>As a (role)</strong></td><td><strong>Users Request  &amp need </strong></td><td><strong>So the user should know &amp he does enough activity again.:thermometer: (user value)</strong></td><td><strong>Acceptance Criteria</strong></td></tr><tr><td><strong>1</strong></td><td>Exercise enthusiast</td><td>I want to track my steps</td><td>To ensure I get enough activity</td><td>A Power BI dashboard <br>which lets me get an<br>easy and quick overview of my exercise data.</td></tr></tbody></table>


<h2>Data Collection &amp; Table Structures</h2>
<hr class="wp-block-separator is-style-wide">


<p>The necessary data were collected and structured in Excel files. The exercise data was organized as a fact table and date &amp; activity were organized as dimension tables for filtering data.</p>




<table> ❔ Asked The Question's at Initial Stage 

<tr>	
	<td>
		What are the requirements to gather the fitbit data, and in order to analyse what?
	</td>
	<td>
		To know What are our activities, and is that activity enough to burn the required calories sustantialy.
	</td>
	<td> 
		To do discriptive analysis The time of week, my activity is at most
	</td>
	<td>
		To do predictive analysis to know what will be the required activity by catagories such as walking and running
	</td>
	<td>
		Analyzing the negative factors affecting which hinders consistency in porformance growth like any (injury)</td>
</tr>
</table>

<p><strong>:heavy_exclamation_mark: Fact Exercise</strong></p>

<p>Exercise data were recorded every single date and the focus was on amount of steps. The date column is used to connect to the date dimension and Activity_FK is used to connect to the activity dimension.</p>


<img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data.png?w=300g">

<p>Following steps were done in Power BI to transform this table to be ready for analysis purposes:</p>

<ol><li>Promoted row so that the data so that the first row was used as headers.</li><li>Removed unnecessary columns.</li><li>Changed column to have the correct type (date, numbers etc.) for later use in calculations.</li></ol>



<figure class="wp-block-image size-large is-style-default"><img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image.png?w=277" alt="" class="wp-image-228" ></figure>



<p><strong>:heavy_exclamation_mark:Dim_Activity</strong></p>



<p>DIM_Activity describes two different types of activities: Walking and running. On some days walking was chosen as a preferred activity time, and other days running were performed. Some minor data issues in this table was later cleaned up and corrected.</p>



<figure class="wp-block-image <img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data-2.png?w=714" sizes="(max-width: 714px) 100vw, 714px"></figure>



<p> Following steps were done in Power BI to transform this table to be ready for analysis purposes: </p>



<ol><li>Promoted row so that the data so that the first row was used.</li><li>Renamed necessary columns to give better business friendly names.</li><li>Capitalized each for in the description column for improved data quality.</li></ol>



<img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-1.png">



<p><strong>:heavy_exclamation_mark:DIM_Date</strong></p>



<p>The DIM_Date dimension is based on a simple table with dates, where date was used to derive several new fields which would be used in the exercise analysis dashboard:</p>



<ol><li>Promoted row so that the data so that the first row was used.</li><li>Changed the column to DateType</li><li>Inserted several new columns based on the date.</li></ol>



<img src=https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-2.png">

<p></p>



<hr class="wp-block-separator is-style-wide">



<h2>Data Model</h2>



<p>Below is a screenshot of the data model after cleansed and prepared tables were read into Power BI.</p>



<p>We can see that the FACT table is connected to two dimension tables with the correct relationship established (1 to *) between dimension and fact tables.</p>



<figure class="wp-block-image size-large is-style-default"><img src ="https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model-1.png" 



<hr class="wp-block-separator is-style-wide">



<h2>Calculations</h2>



<p><h5>The following calculations were created in the Power BI reports using DAX (Data Analysis Expressions). To lessen the extent of coding, the re-use of measures (measure branching) was emphasized:</h5></p>



<p><strong>Average Steps</strong> – This is a simple AVERAGE function around the Steps column:<br>
	
```	
	AVERAGE( FACT_Activity[Steps] )
```


<p><strong>Total Steps</strong> – This is a simple SUM function around the Steps column: 
	
```
	SUM( FACT_Activity[Steps] )</p>
```


<p><strong>Steps (Running)</strong> – This is a calculation to isolate the Total Steps measure by filtering it by the “Running Activity”:<br></p>
	
```	CALCULATE
	(
	[Total Steps],DIM_Activity[ActivityName] = “Running”
	)
```	
   

<p><strong>Steps (Walking)</strong>   – This is a calculation to isolate the Total Steps measure by filtering it by the “Walking Activity”:<br></p>
	
```	
	CALCULATE
	(
	[Total Steps], DIM_Activity[ActivityName] = “Running”
	)
```
<p><strong>Steps (Walking)</strong>   – This is a calculation to isolate the Total Steps measure by filtering it by the “Walking Activity”:<br></p>```	CALCULATE
```	CALCULATE
	(
	[Total Steps], DIM_Activity[ActivityName] = “Walking”
	)
```

<p> <strong>Running % of Total</strong> – Here we are using two measures from before to find the % of steps that were done by running:<br></p>
	
```	
	DIVIDE
	(
	[Steps (Running)], [Total Steps]
	) 
```


<p> <strong>Walking % of Total</strong>  – Here we are using two measures from before to find the % of steps that were done by walking: <br></p>
	
```	DIVIDE
	(
	[Steps (Walking)], [Total Steps]
	) 
```

<p><strong>Total Steps (Cumulative)</strong> – Here we are re-using the Total Steps measure and using different functions to cumulatively calculate the total steps:<br></p>
	
```	CALCULATE
	(
	[Total Steps],FILTER ( ALLSELECTED ( DIM_Date ), DIM_Date[Date]&lt;= MAX( FACT_Activity[Date] ))
	)
```


<p><strong>Week Over Week % Change Steps</strong> – Here we are using the Total Steps measure and using different functions, with variables, to calculate the Week over Week % Change of Steps:<br></p>
	
```	
	VAR CurrentWeek = CALCULATE
	(
		[Total Steps],FILTER(ALL( DIM_Date ),
		DIM_Date[Week of Year] = SELECTEDVALUE( DIM_Date[Week of Year] ))
	)

```
		VAR PreviousWeek = CALCULATE
		(
			[Total Steps],
			FILTER
			(ALL( DIM_Date ),
			DIM_Date[Week of Year] = SELECTEDVALUE( DIM_Date[Week of Year] ) – 1)
		)
		RETURN DIVIDE(( CurrentWeek – PreviousWeek ), PreviousWeek )'''



<hr class="wp-block-separator is-style-wide">



<p></p>



<h2>Exercise Analysis Dashboard</h2>



<p>The finish report consists of two different dashboards. One is more of a basic version, while the second version contains more advanced visualizations. To enable these visualizations the calculation language DAX (Data Analysis Expressions) were used.</p>



<p><strong>Click the picture to to open the dashboard and try it out!</strong></p>



<p><strong>Basic Version:</strong></p>



<!--<figure class="wp-block-image size-large is-style-default"><a href=""><img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png?w=1024"> </a></figure>-->



<p><strong>Advanced Version:</strong></p>



 <figure> <a href="" <img  src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png?w=1024"</a></figure>
 <!--.content-wrapper -->

<!-- .social link-wrapper -->
<div class="menu"><ul id="menu-social">
<li class="menu-item menu-item-type-custom menu-item-object-custom menu-item-25"><a href="https://www.linkedin.com/in/karan-shah-020b4baa"><span class="screen-reader-text">Instagram</span><svg class="icon icon-instagram" aria-hidden="true" role="img"> <use href="#icon-instagram" xlink:href="#icon-instagram"></use> </svg></a></li>
<li class="menu-item menu-item-type-custom menu-item-object-custom menu-item-47"><a href="https://www.instagram.com/karanzshah/"><span class="screen-reader-text">LinkedIn</span><svg class="icon icon-linkedin" aria-hidden="true" role="img"> <use href="#icon-linkedin" xlink:href="#icon-linkedin"></use> </svg></a></li>
</ul></div>

  
