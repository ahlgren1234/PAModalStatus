# PAModalStatusView

Create an PA Modal Status View for light actions in iOS Apps.

PA Modal Status View is a framework created to recreate Apple's private Modal Status View. 

While designing iOS apps we may want to alert the user to a successful completion of a task.
Many different methods have arrived to do just this, from a subtle drop down notification covering the status bar to a more interfering UIAlertView.

Apple's solution is to display a self-removing and small modal view to the screen.

![text](https://user-images.githubusercontent.com/20458718/31577957-33ec53ce-b0dd-11e7-8b50-0031889040fd.PNG "Apple's custom use of Modal Status Views")

With uses in the News app, the Apple Music app, and the Podcasts app, developers have been wanting access to this view for a while now. 
That is what this framework solves.

## Design

<img src="https://github.com/ahlgren1234/PAModalStatus/blob/master/screenshot.jpg?raw=true" width="250px" />

## Instructions

Simply import the framework and add the following code to get started.

    let modalView = PAModalStatusView(frame: self.view.bounds)
    view.addSubview(modalView)

Further customize the PAModalStatusView with the following functions:

    modalView.set(image: successImage)
    modalView.set(headline: "Alright!")
    modalView.set(subheading: "Working great!")
