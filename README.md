## **BMICalculatorMAUI**

An MVVM focused project led by Hector Perez on his Udemy course: *.NET MAUI course with Visual Studio 2022 creating PROJECTS*

The UI for this application is cleverly built out with *Syncfusion* 'gauges', allowing for a more visually satisfying look. The View is broken down into 3 portions: *Height*, *Weight*, and *Result*. Both *Height* and *Weight* implement *LinearGauges* with Sliders that update their own values and the *Result* value when the Sliders are moved. *Result* utilizes a *RadialGauge* broken down into each of the BMI categories that has a Pointer that updates with each of the Sliders, and has a Label that displays the BMI category dynamically.

The ViewModel simply implements the *BMI* Class to be used in the View. 
The *BMI* Model utilizes the *PropertyChanged.Fody* NuGet Package. This INCREDIBLY nifty Package adds the *INotifyPropertyChanged* Interface to a Class without actually requiring full implementation of the Interface itself. In doing so, a lot of code is spared from being written, which in turn makes the Class a much cleaner read. 
