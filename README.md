# AspNetBootStrapFix
How to fix the 'Nav-Bar' problem after updating Nugets to BootStrap 4.0+

- Install and register 'FontAwesome' as shown in adjacent sections
	- Download 'FontAwesome' Nuget and install via package manager
	- Add 'FontAwesome' css and js files as Bundle in 'BundleConfig'
	- Add 'FontAwesome' css and js files as Bundle in 'BundleConfig'
	- Register 'FontAwesome' Bundle in the _Layout/.cshtml

- Modify the '_Layout.cshtml' - 'Nav-Bar div' html with code displayed at bottom:

BootStrap 4.0+ Nav-Bar HTML Source:

	<div class="navbar navbar-expand-sm navbar-dark fixed-top bg-dark">
		<div class="container">
			<div class="navbar-header">
				<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
					<i class="fas fa-bars"></i>
				</button>
				<a class="navbar-brand" href="/">Ebille</a>
			</div>
			<div class="navbar-collapse collapse" id="navbarSupportedContent">
				<ul class="nav navbar-nav mr-auto">
					<li class="nav-item"><a class="nav-link" href="/">Home</a></li>
					<li class="nav-item"><a class="nav-link" href="/Help">API</a></li>
				</ul>
			</div>
		</div>
	</div>

- Make changes to the 'ActionLink' as per your requirmentsBootStrap 4.0+ Nav-Bar HTML: