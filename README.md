<h2>rappidDASH</h2>

<h5><span class="note">Dashboard and component framework - <em>just enough to be helpful and not a hassle </em></h5>


<br><br>
<b><big>
	GET STARTED IN LESS THAN A MINUTE:
	</big></b>

<b>CSS includes: place in head section of HTML page</b>
Bootstrap 3 css: 

<b>Javascript includes: place at bottom of HTML body</b><br>
<br>
BOOTSTRAP: <br>
JQUERY: <br>
RAPIDDASH:<br>
RAPIDCONTROL:<br>
<br>
.. INCLUDE ANY OTHER CONNTROLS refs YOU WISH TO USE ON YOUR DASH
<br><br>

<b>HTML: Add rapidcontrols anywhere you want them on web page</b><br><br>
<br>
<b>DASHBOARD</b>: this html is the dashboard. Place anything you want on the dashboard inside this wrapper.
<br>

<code>
	
	<div id="MyDashboardId" class="rapiddash-control rdDashlet" data-display="normal" data-controlType="rdDashlet" data-contentType="inline"> ... dashboard elements here </div>
	
	
	</code>
	
	
	<br>
Here are a few examples of rapid controls you can incude in your dashboard. Add as many as you wish. be sure to include js files for any rapid cotrols you use.<br><br>

<b>BASIC PORTLET</b> : Genereic control to wrap around any content you want to turn into a portlet on your dash.
<br><br>
<code>
	
	
	<div id="MySImpleTextPortlet" class="rapiddash-control" data-controlType="rdDashlet" data-display="normal" data-contentType="inline">
	   ... here is some random text that will appear in my sexy portlet ...	</div>
	
	
	</code>
	
<br><br>


PORTLET WITH LINKED CONTENT: You'll probably want to link to the content for most of your dashlets - it is cleaner and required for most of the more dynamic control types.<br><br>

<code>
	
	<div id="myLinkList" class="rapiddash-control" data-controlType="rdDashlet" data-display="noral" data-contentType="linked" data-source="myCOntentFilesPath/MyLinkListFile.htm"-></div>
	</code>
	
	<br><br>

<b>LAST STEP</b>: INCLUDE THIS SCRIPT CODE ANYWHERE ON ANY PAGE CONTAINING A RAPIDDASH.

<br><br>


<code>
<script>
	
	$(document).ready(function(){
		rapidDash.init();
	}) ;
	
</script>
	
</code>

<br><br><br>


<p><strong><u>components:</u></strong></p>

 <div class="formattedExport">
<ul>
	<li><span class="name">Panel Templates - content files that load into rapidlets</span>
	<ul>
		<li><span class="name">model dialogues with embedded bootstrap panels</span></li>
		<li><span class="name">bootstrap panels</span></li>
	</ul>
	</li>
	<li><span class="name"><u><strong>Contrrol Types</strong></u></span>
	<ul>
		<li><span class="name"><strong>RAPIdDASH </strong>- parent wrapper and control for dashboard</span></li>
		<li><span class="name"><strong>DASHLETS</strong>- portlet that dynamically load - can only go in dashletgroup wrapper</span>
		<ul>
			<li><span class="name">modal - not displayed until triggered by link</span></li>
			<li><span class="name">expandable - title displayed and content rendered when expanded</span></li>
			<li><span class="name">normal - normal portlet container loads inline on parent page loadCommand panel - top level navigation and headings</span></li>
		</ul>
		</li>
		<li><span class="name"><strong>Control Group</strong>- wrapper and controller for group of controls</span>
		<ul>
			<li><span class="name">containers for controls</span></li>
			<li><span class="name">responsible for initializing controls within</span></li>
			<li><span class="name">properties</span>
			<ul>
				<li><span class="name">default Active Control -none | id of control to be active on load</span></li>
				<li><span class="name">control Display Type - Single | multiple</span></li>
				<li><span class="name">definition File - optional path to JSON Definition</span></li>
			</ul>
			</li>
		</ul>
		</li>
		<li><span class="name"><strong>Contentlet </strong>- editable HTML content snippets</span>
		<ul>
			<li><span class="name">partlet - specialized controls that can be included within contenlets</span>
			<ul>
				<li><span class="name">Filelet - link list of files of specified type in specified directory</span></li>
				<li><span class="name">Linklet- editable list of hyperlinks</span></li>
			</ul>
			</li>
		</ul>
		</li>
		<li><span class="name"><strong>Commandlet </strong>- button panel</span></li>
		<li><span class="name"><strong>Runlet </strong>- generic portlet that call specified function and inserts returned HTML into specified element</span></li>
		<li><span class="name"><strong>Reportlet </strong>- reports that can be expanded/contracted/refreshed on dashboard - reports built automatically from either a SQL statement or json definition</span></li>
		<li><span class="name"><strong>Formlet </strong>- generates input form for database records and displays database records. automatically generates insert and update SQL</span></li>
	</ul>
	</li>
</ul>

<p> </p>

<ul>
	<li><strong><span class="name">Page STRUCTURE</span></strong><ul><li><span class="name">rapiddsh </span>
<ul>
		<li><span class="name">control group</span>
<ul>
				<li><span class="name">Dashlets</span>
<ul>
				<li><span class="name">control groups</span></li>
				</ul>
				</li>
			</ul>
			</li>
		</ul>
		</li>
	</ul>
	</li>
</ul>

<p> </p>

<ul>
	<li><strong><span class="name">EXAMPLE dashbord ...</span></strong><ul>
		<li><span class="name">MY DASHBOARD - rapiddash control</span>
<ul><li><span class="name">Left column portlets - control group control to wrap controls</span>
<ul>
	<li><span class="name">My data manager 1 - rapidlet loads specified file</span>
<ul>
			<li><span class="name">My data 1 components - control group to wrap controls</span></li>
					<li><span class="name">List of records in Oracle Table 1 - reportlet control to display data records</span></li>
					<li><span class="name">Add new record form 1 - custom formlet control to add/display record data</span></li>
				</ul>
				</li>
				<li><span class="name">My Recommended Links - rapidlet control 2 - loads link list 1 file</span>
				<ul>
					<li><span class="name">panel group - container for link list control</span>
					<ul>
						<li><span class="name">linklist 1 - custom control to display and manage list of hyperlinks</span></li>
					</ul>
					</li>
				</ul>
				</li>
				<li><span class="name">rapidlet control 3 ...</span>
				<ul>
					<li><span class="name">...</span></li>
				</ul>
				</li>
			</ul>
			</li>
			<li><span class="name">panel group 2</span>
			<ul>
				<li><span class="name">...</span></li>
			</ul>
			</li>
		</ul>
		</li>
	</ul>
	</li>
</ul>
</div>
