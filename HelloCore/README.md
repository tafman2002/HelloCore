# ASP.NET Core Project
This project contains a simple MVC application written in C#.

## Model - View - Controller (MVC)
- Model represents the shape of the data
- View represents the user interface
- Controller handles the user request and acts as an interface between Model and View

By convention, the directories in view will have the same name as the corresponding controller
with the ending having Controller e.g Home <-> HomeController.

## Routing
Similar to Next JS structure, the public methods in Controllers correspond to the page routing in browsers. Example:
```
 public HomeController(ILogger<HomeController> logger) {
     // This is /home/index
     public IActionResult Index()
        {
            return View();
        }

    // This is /home/privacy
     public IActionResult Privacy()
        {
            return View();
        }
 }
```

## Tag Helpers
Tag Helpers enable server-side code to participate in creating and rendering
HTML elements in Razor files.
