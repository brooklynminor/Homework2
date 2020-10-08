Brooklyn Minor
# Homework 2: Portfolio
The purpose of this project was to implement Bootstrap elements into an html file and manipulate the display using CSS to our own discretion.
Three files were made separately: Portfolio.html, AboutMe.html and ContactInformation.html. Each of the aforementioned files contain CSS and JavaScript depending on the finale display of the webpage. 
Each page allows access to one another through the toggle icon in the navigation bar. JavaScript was added to run those functions. An onclick function is inserted into the button tag to define the event. 
```
           <nav class="navbar navbar-dark bg-dark">
                <a class="navbar-brand" href="#">Brooklyn Minor</a>
                <button class="navbar-toggler" onclick="myClick()" type="button" data-toggle="collapse" data-target="#navbarToggleExternalContent" aria-controls="navbarToggleExternalContent" aria-expanded="false" aria-label="Toggle navigation" style="text-align: left; float: left; left: 20px">
                <span class="navbar-toggler-icon"></span>
            </button>
            </nav>
            <div class="navbar-toggler-icon-content" id="myDropdown">
                <a class="nav-link" href="AboutMe.html">About Me</a>
                <a class="nav-link" href="Portfolio.html">Portfolio</a>
                <a class="nav-link" href="ContactInformation.html">Contact Information</a>
            </div>
        </div>
    </div>
```
The grid system is used to organize the page layout. Containers provide a pad around the files content. Rows wrap columns horizontally, well padding controls the spacing between each element. Content is placed within column classes which indicate the number of columns used (12 columns per row). 
Each webpage was designed to be accessible when viewing from different devices by implementing the grid system within the html files. Breakpoints are used based on the width of the media query. In this case, sm was used for devices ≥576px.  
```
<div class="container-fluid">
        <div class="row">
            <div class="col-sm-3">
                <img src="https://via.placeholder.com/200x200.png?text=200x200" class="card-img-top" alt="200x200">
            </div>
            <div class="col-sm-5">
                <h2>About Me</h2>
```
On the About Me page in the second row, along the left-hand side contains a card with links that will redirect the user to the page listed.
```
             <div class="col-sm-2">
              <div class="card" style="width: 18rem;">
                <div class="card-header">
                  Networking
                </div>
                <ul class="list-group list-group-flush">
                  <li class="nav-link" onclick="myLinkedIn()"href="https://www.linkedin.com/in/brooklyn-minor-742245109/">LinkedIn</li>
                  <li class="nav-link" onclick="myGitHub()" href="https://github.com/brooklynminor">GitHub</li>
                  <li class="nav-link" onclick="myGitLab()" href="https://utoronto.bootcampcontent.com/brooklynminor">Gitlab</li>
                </ul>
              </div>
            </div>
          </div>
```
 JavaScript was added to the html file to redirect users when the element is clicked, this occurs through an onclick function. 
```    function myLinkedIn() {
  location.replace("https://www.linkedin.com/in/brooklyn-minor-742245109/")
}
   function myGitHub() {
  location.replace("https://github.com/brooklynminor")
}
    function myGitLab() {
  location.replace("https://utoronto.bootcampcontent.com/brooklynminor")
}
```
The file is pushed to the repository through GitBash
