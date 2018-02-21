<h2>rappiDASH</h2>

<h5><em><span class="note">Dashboard and component framework</em></h5>

<div> </div>

<p><strong><u>Architecture:</u></strong></p>



<ul>
	<li><strong>Dashboard </strong >page - object - related code files
	<ul>
		<li><strong>Command pane</strong>l - top level navigation and headings</li>
		<li><strong>dashlets </strong>- portlets that can be mixed and matched for a dashboard
		<ul>
			<li><strong>Contentlet </strong>- editable HTML content snippets
			<ul>
				<li><strong>partlet </strong>- specialized controls that can be included within contenlets
				<ul>
					<li><strong>Filelet </strong>- link list of files of specified type in specified directory</li>
					<li><strong>Linklet</strong>- editable list of hyperlinks</li>
				</ul>
				</li>
			</ul>
			</li>
			<li><strong>Commandlet </strong>- button panel</li>
			<li><strong>Runlet </strong>- generic portlet that call specified function and inserts returned HTML into specified element</li>
			<li><strong>Reportlet </strong>- reports that can be expanded/contracted/refreshed on dashboard - reports built automatically from either a SQL statement or json definition</li>
			<li><strong>Formlet </strong>- generates input form for database records and displays database records. automatically generates insert and update SQL</li>
			<li><strong>DASHLET</strong> - DATA management portlets 
			<ul>
				<li><em>list view tab</em> - lists data records</li>
				<li><em>record tab</em> - displays single record in form view and for record updating</li>
				<li><em>new input </em>- generates input for for adding new records</li>
			</ul>
			</li>
		</ul>
		</li>
	</ul>
	</li>
</ul>
