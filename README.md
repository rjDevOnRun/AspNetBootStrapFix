# AspNetBootStrapFix
How to fix the 'Nav-Bar' problem after updating Nugets to BootStrap 4.0+

- Install and register 'FontAwesome' as per steps below:
	- Install 'FontAwesome MVC' Nuget to your project
	- Add 'FontAwesome' css and js files as Bundle in 'BundleConfig'
	- Register 'FontAwesome' Bundle in the _Layout/.cshtml

- Modify the '_Layout.cshtml' - 'Nav-Bar div' html with code displayed here:

BootStrap 4.0+ Nav-Bar HTML Source:

	<div class="navbar navbar-expand-sm navbar-dark fixed-top bg-dark">
		<div class="container">
			<div class="navbar-header">
				<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
					<i class="fas fa-bars"></i>
				</button>
				@Html.ActionLink("NavBar", "Index", "Home", new { area = "" }, new { @class = "navbar-brand" })
			</div>
			<div class="navbar-collapse collapse" id="navbarSupportedContent">
				<ul class="nav navbar-nav mr-auto">
					<li class="nav-item">@Html.ActionLink("Home", "Index", "Home", null, new { @class = "nav-link" })</li>
                        		<li class="nav-item">@Html.ActionLink("About", "About", "Home", null, new { @class = "nav-link" })</li>
                        		<li class="nav-item">@Html.ActionLink("Contact", "Contact", "Home", null, new { @class = "nav-link" })</li>
				</ul>
			</div>
		</div>
	</div>

- Make changes to the '@Html.ActionLink' as per your requirmentsBootStrap 4.0+ Nav-Bar HTML:
