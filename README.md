
<div class="site-branding">
										<h1 >Analyze with Karan</h1>
							<p class="site-description">Data Analyst Portfolio Example on Excercise Data Set</p>
			
	
</ul></div>		</nav><!-- .jetpack-social-navigation -->
				</div>
		

	
	

				
<article>
	<header >
		<h1 class="entry-title">Data Analyst Portfolio Project-1 – Exercise Analysis</h1>	</header>
		<div >
			




<div class="wp-block-coblocks-gallery-masonry alignwide"><div class="coblocks-gallery has-caption-style-dark has-gutter"><ul class="has-grid-xlrg has-gutter-15 has-gutter-mobile-15" style="position: relative; height: 309.463px;"><img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/power-bi-applied-steps.png?w=524g"<figure class="coblocks-gallery--figure">
	<li class="coblocks-gallery--item" style="position: relative ; top: 12px;"><figure class="coblocks-gallery--figure"><img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data.png?w=400"<figure class="coblocks-gallery--figure"><img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model.png?w=300g" data-id="217">
	<img src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2.png?w=480?w=400g">
		</li></li></ul></div></div>



<hr class="wp-block-separator is-style-wide">



<h2>Business Request &amp; User Stories </h2>



<p>The business request for this project was created by the user himself. By deciding on a business to analyze (exercise data) the following user story was derived.</p>



<figure class="wp-block-table is-style-stripes"><table><tbody><tr><td><strong> #</strong></td><td><strong>As a (role)</strong></td><td><strong>I want (request / demand)</strong></td><td><strong>So that I (user value)</strong></td><td><strong>Acceptance Criteria</strong></td></tr><tr><td><strong>1</strong></td><td>Exercise enthusiast</td><td>I want to track my steps</td><td>To ensure I get enough activity</td><td>A Power BI dashboard <br>which lets me get an<br>easy and quick overview of my exercise data.</td></tr></tbody></table></figure>



<p></p>
</div>
</div>



<h2>Data Collection &amp; Table Structures</h2>



<p>The necessary data were collected and structured in Excel files. The exercise data was organized as a fact table and date &amp; activity were organized as dimension tables for filtering data.</p>



<p><strong>FACT_ Exercise</strong></p>



<p>Exercise data were recorded every single date and the focus was on amount of steps. The date column is used to connect to the date dimension and Activity_FK is used to connect to the activity dimension.</p>



<figure class="wp-block-image size-large is-style-default"><img data-attachment-id="217" data-permalink="https://analyzewithaliportfolio.wordpress.com/raw-data/" data-orig-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data.png" data-orig-size="455,576" data-comments-opened="1" data-image-meta="{&quot;aperture&quot;:&quot;0&quot;,&quot;credit&quot;:&quot;&quot;,&quot;camera&quot;:&quot;&quot;,&quot;caption&quot;:&quot;&quot;,&quot;created_timestamp&quot;:&quot;0&quot;,&quot;copyright&quot;:&quot;&quot;,&quot;focal_length&quot;:&quot;0&quot;,&quot;iso&quot;:&quot;0&quot;,&quot;shutter_speed&quot;:&quot;0&quot;,&quot;title&quot;:&quot;&quot;,&quot;orientation&quot;:&quot;0&quot;}" data-image-title="raw-data" data-image-description="" data-medium-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data.png?w=300"></figure>



<p>Following steps were done in Power BI to transform this table to be ready for analysis purposes:</p>



<ol><li>Promoted row so that the data so that the first row was used as headers.</li><li>Removed unnecessary columns.</li><li>Changed column to have the correct type (date, numbers etc.) for later use in calculations.</li></ol>



<figure class="wp-block-image size-large is-style-default"><img data-attachment-id="228" data-permalink="https://analyzewithaliportfolio.wordpress.com/image/" data-orig-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image.png" data-orig-size="277,297" data-comments-opened="1" data-image-meta="{&quot;aperture&quot;:&quot;0&quot;,&quot;credit&quot;:&quot;&quot;,&quot;camera&quot;:&quot;&quot;,&quot;caption&quot;:&quot;&quot;,&quot;created_timestamp&quot;:&quot;0&quot;,&quot;copyright&quot;:&quot;&quot;,&quot;focal_length&quot;:&quot;0&quot;,&quot;iso&quot;:&quot;0&quot;,&quot;shutter_speed&quot;:&quot;0&quot;,&quot;title&quot;:&quot;&quot;,&quot;orientation&quot;:&quot;0&quot;}" data-image-title="image" data-image-description="" data-medium-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image.png?w=277" data-large-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image.png?w=277" src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image.png?w=277" alt="" class="wp-image-228" srcset="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image.png 277w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/image.png?w=140 140w" sizes="(max-width: 277px) 100vw, 277px"></figure>



<p><strong>DIM_Activity</strong></p>



<p>DIM_Activity describes two different types of activities: Walking and running. On some days walking was chosen as a preferred activity time, and other days running were performed. Some minor data issues in this table was later cleaned up and corrected.</p>



<figure class="wp-block-image size-large is-style-default"><img data-attachment-id="225" data-permalink="https://analyzewithaliportfolio.wordpress.com/raw-data-2/" data-orig-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data-2.png" data-orig-size="714,666" data-comments-opened="1" data-image-meta="{&quot;aperture&quot;:&quot;0&quot;,&quot;credit&quot;:&quot;&quot;,&quot;camera&quot;:&quot;&quot;,&quot;caption&quot;:&quot;&quot;,&quot;created_timestamp&quot;:&quot;0&quot;,&quot;copyright&quot;:&quot;&quot;,&quot;focal_length&quot;:&quot;0&quot;,&quot;iso&quot;:&quot;0&quot;,&quot;shutter_speed&quot;:&quot;0&quot;,&quot;title&quot;:&quot;&quot;,&quot;orientation&quot;:&quot;0&quot;}" data-image-title="raw-data-2" data-image-description="" data-medium-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data-2.png?w=300" data-large-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data-2.png?w=714" src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data-2.png?w=714" alt="" class="wp-image-225" srcset="https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data-2.png 714w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data-2.png?w=150 150w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/raw-data-2.png?w=300 300w" sizes="(max-width: 714px) 100vw, 714px"></figure>



<p> Following steps were done in Power BI to transform this table to be ready for analysis purposes: </p>



<ol><li>Promoted row so that the data so that the first row was used.</li><li>Renamed necessary columns to give better business friendly names.</li><li>Capitalized each for in the description column for improved data quality.</li></ol>



<figure class="wp-block-image size-large is-style-default"><img data-attachment-id="230" data-permalink="https://analyzewithaliportfolio.wordpress.com/image-1/" data-orig-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-1.png" data-orig-size="269,291" data-comments-opened="1" data-image-meta="{&quot;aperture&quot;:&quot;0&quot;,&quot;credit&quot;:&quot;&quot;,&quot;camera&quot;:&quot;&quot;,&quot;caption&quot;:&quot;&quot;,&quot;created_timestamp&quot;:&quot;0&quot;,&quot;copyright&quot;:&quot;&quot;,&quot;focal_length&quot;:&quot;0&quot;,&quot;iso&quot;:&quot;0&quot;,&quot;shutter_speed&quot;:&quot;0&quot;,&quot;title&quot;:&quot;&quot;,&quot;orientation&quot;:&quot;0&quot;}" data-image-title="image-1" data-image-description="" data-medium-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-1.png?w=269" data-large-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-1.png?w=269" src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-1.png?w=269" alt="" class="wp-image-230" srcset="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-1.png 269w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-1.png?w=139 139w" sizes="(max-width: 269px) 100vw, 269px"></figure>



<p><strong>DIM_Date</strong></p>



<p>The DIM_Date dimension is based on a simple table with dates, where date was used to derive several new fields which would be used in the exercise analysis dashboard:</p>



<ol><li>Promoted row so that the data so that the first row was used.</li><li>Changed the column to DateType</li><li>Inserted several new columns based on the date.</li></ol>



<figure class="wp-block-image size-large is-style-default"><img data-attachment-id="233" data-permalink="https://analyzewithaliportfolio.wordpress.com/image-2/" data-orig-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-2.png" data-orig-size="278,354" data-comments-opened="1" data-image-meta="{&quot;aperture&quot;:&quot;0&quot;,&quot;credit&quot;:&quot;&quot;,&quot;camera&quot;:&quot;&quot;,&quot;caption&quot;:&quot;&quot;,&quot;created_timestamp&quot;:&quot;0&quot;,&quot;copyright&quot;:&quot;&quot;,&quot;focal_length&quot;:&quot;0&quot;,&quot;iso&quot;:&quot;0&quot;,&quot;shutter_speed&quot;:&quot;0&quot;,&quot;title&quot;:&quot;&quot;,&quot;orientation&quot;:&quot;0&quot;}" data-image-title="image-2" data-image-description="" data-medium-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-2.png?w=236" data-large-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-2.png?w=278" src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-2.png?w=278" alt="" class="wp-image-233" srcset="https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-2.png 278w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/image-2.png?w=118 118w" sizes="(max-width: 278px) 100vw, 278px"></figure>



<p></p>



<hr class="wp-block-separator is-style-wide">



<h2>Data Model</h2>



<p>Below is a screenshot of the data model after cleansed and prepared tables were read into Power BI.</p>



<p>We can see that the FACT table is connected to two dimension tables with the correct relationship established (1 to *) between dimension and fact tables.</p>



<figure class="wp-block-image size-large is-style-default"><img data-attachment-id="234" data-permalink="https://analyzewithaliportfolio.wordpress.com/data-model-1/" data-orig-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model-1.png" data-orig-size="787,699" data-comments-opened="1" data-image-meta="{&quot;aperture&quot;:&quot;0&quot;,&quot;credit&quot;:&quot;&quot;,&quot;camera&quot;:&quot;&quot;,&quot;caption&quot;:&quot;&quot;,&quot;created_timestamp&quot;:&quot;0&quot;,&quot;copyright&quot;:&quot;&quot;,&quot;focal_length&quot;:&quot;0&quot;,&quot;iso&quot;:&quot;0&quot;,&quot;shutter_speed&quot;:&quot;0&quot;,&quot;title&quot;:&quot;&quot;,&quot;orientation&quot;:&quot;0&quot;}" data-image-title="data-model-1" data-image-description="" data-medium-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model-1.png?w=300" data-large-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model-1.png?w=787" src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model-1.png?w=787" alt="" class="wp-image-234" srcset="https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model-1.png 787w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model-1.png?w=150 150w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model-1.png?w=300 300w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/data-model-1.png?w=768 768w" sizes="(max-width: 787px) 100vw, 787px"></figure>



<hr class="wp-block-separator is-style-wide">



<h2>Calculations</h2>



<p>The following calculations were created in the Power BI reports using DAX (Data Analysis Expressions). To lessen the extent of coding, the re-use of measures (measure branching) was emphasized:</p>



<p><strong>Average Steps</strong> – This is a simple AVERAGE function around the Steps column:<br>AVERAGE( FACT_Activity[Steps] )</p>



<p><strong>Total Steps</strong> – This is a simple SUM function around the Steps column:<br>SUM( FACT_Activity[Steps] )</p>



<p><strong>Steps (Running)</strong> – This is a calculation to isolate the Total Steps measure by filtering it by the “Running Activity”:<br><br>CALCULATE(<br>[Total Steps],<br>DIM_Activity[ActivityName] = “Running”<br>)</p>
     


<p><strong>Steps (Walking)</strong>   – This is a calculation to isolate the Total Steps measure by filtering it by the “Walking Activity”:<br><br>CALCULATE(<br>[Total Steps],<br>DIM_Activity[ActivityName] = “Walking”<br>)</p>



<p> <strong>Running % of Total</strong> – Here we are using two measures from before to find the % of steps that were done by running:<br><br>DIVIDE(<br>[Steps (Running)],<br>[Total Steps]<br>) </p>



<p> <strong>Walking % of Total</strong>  – Here we are using two measures from before to find the % of steps that were done by walking: <br><br>DIVIDE(<br>[Steps (Walking)],<br>[Total Steps]<br>) </p>



<p><strong>Total Steps (Cumulative)</strong> – Here we are re-using the Total Steps measure and using different functions to cumulatively calculate the total steps:<br><br>CALCULATE(<br>[Total Steps],<br>FILTER(<br>ALLSELECTED( DIM_Date ),<br>DIM_Date[Date]<br>&lt;= MAX( FACT_Activity[Date] )<br>)<br>)</p>



<p><strong>Week Over Week % Change Steps</strong> – Here we are using the Total Steps measure and using different functions, with variables, to calculate the Week over Week % Change of Steps:<br><br>VAR CurrentWeek =<br>CALCULATE(<br>[Total Steps],<br>FILTER(<br>ALL( DIM_Date ),<br>DIM_Date[Week of Year]<br>= SELECTEDVALUE( DIM_Date[Week of Year] )<br>)<br>)<br>VAR PreviousWeek =<br>CALCULATE(<br>[Total Steps],<br>FILTER(<br>ALL( DIM_Date ),<br>DIM_Date[Week of Year]<br>= SELECTEDVALUE( DIM_Date[Week of Year] ) – 1<br>)<br>)<br>RETURN<br>DIVIDE(<br>( CurrentWeek – PreviousWeek ),<br>PreviousWeek<br>)<br></p>



<hr class="wp-block-separator is-style-wide">



<p></p>



<h2>Exercise Analysis Dashboard</h2>



<p>The finish report consists of two different dashboards. One is more of a basic version, while the second version contains more advanced visualizations. To enable these visualizations the calculation language DAX (Data Analysis Expressions) were used.</p>



<p><strong>Click the picture to to open the dashboard and try it out!</strong></p>



<p><strong>Basic Version:</strong></p>



<figure class="wp-block-image size-large is-style-default"><a href="https://app.powerbi.com/view?r=eyJrIjoiYTU3ZTFhZjgtNTY3ZC00MWI1LWE1YmYtMTU1OTQxOTIyMjFjIiwidCI6IjMzYTJhMWQwLTI1MDgtNGJkNC05M2Y0LWRlYmRhMDM1MmFmYyIsImMiOjh9" target="_blank"><img data-attachment-id="236" data-permalink="https://analyzewithaliportfolio.wordpress.com/dashboard-1-2/" data-orig-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png" data-orig-size="1920,1019" data-comments-opened="1" data-image-meta="{&quot;aperture&quot;:&quot;0&quot;,&quot;credit&quot;:&quot;&quot;,&quot;camera&quot;:&quot;&quot;,&quot;caption&quot;:&quot;&quot;,&quot;created_timestamp&quot;:&quot;0&quot;,&quot;copyright&quot;:&quot;&quot;,&quot;focal_length&quot;:&quot;0&quot;,&quot;iso&quot;:&quot;0&quot;,&quot;shutter_speed&quot;:&quot;0&quot;,&quot;title&quot;:&quot;&quot;,&quot;orientation&quot;:&quot;0&quot;}" data-image-title="dashboard-1" data-image-description="" data-medium-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png?w=300" data-large-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png?w=825" src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png?w=1024" alt="" class="wp-image-236" srcset="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png?w=1024 1024w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png?w=150 150w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png?w=300 300w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png?w=768 768w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-1.png 1920w" sizes="(max-width: 1024px) 100vw, 1024px"></a></figure>



<p><strong>Advanced Version:</strong></p>



<figure class="wp-block-image size-large is-style-default"><img data-attachment-id="238" data-permalink="https://analyzewithaliportfolio.wordpress.com/dashboard-2-1/" data-orig-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png" data-orig-size="1920,1021" data-comments-opened="1" data-image-meta="{&quot;aperture&quot;:&quot;0&quot;,&quot;credit&quot;:&quot;&quot;,&quot;camera&quot;:&quot;&quot;,&quot;caption&quot;:&quot;&quot;,&quot;created_timestamp&quot;:&quot;0&quot;,&quot;copyright&quot;:&quot;&quot;,&quot;focal_length&quot;:&quot;0&quot;,&quot;iso&quot;:&quot;0&quot;,&quot;shutter_speed&quot;:&quot;0&quot;,&quot;title&quot;:&quot;&quot;,&quot;orientation&quot;:&quot;0&quot;}" data-image-title="dashboard-2-1" data-image-description="" data-medium-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png?w=300" data-large-file="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png?w=825" src="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png?w=1024" alt="" class="wp-image-238" srcset="https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png?w=1024 1024w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png?w=150 150w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png?w=300 300w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png?w=768 768w, https://analyzewithaliportfolio.files.wordpress.com/2021/05/dashboard-2-1.png 1920w" sizes="(max-width: 740px) 100vw, 1024px"></figure>
<!-- .content-wrapper -->

  
