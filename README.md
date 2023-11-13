# homework2
We define a class named GreetingWidget that extends StatelessWidget. This means that this widget is immutable and won't change over time. The widget is designed to display a greeting message. The GreetingWidget is a reusable stateless widget responsible for displaying a greeting message in a stylized way.
MyApp widget  defines the overall structure using a Scaffold, an AppBar, and a centered Column containing instances of the GreetingWidget. main class calls 'runApp' and passes an instance of CounterApp to start the application.

CounterApp class represents the main application widget and extends StatefulWidget.
The createState method is overridden to create an instance of the private _CounterAppState class.
_CounterAppState is the state class for CounterApp, extending State. It contains mutable data and is responsible for updating the UI._counter is an integer variable representing the counter value.
The _incrementCounter method increments the counter and triggers a UI update using the setState method.
The build method returns a MaterialApp widget with a Scaffold. The Scaffold contains an AppBar at the top, a Column in the body with two Text widgets displaying the counter value, and a FloatingActionButton that triggers the _incrementCounter method when pressed.
MyApp2 is a stateless widget, representing the main application widget. We build method returns a MaterialApp with a Scaffold. The Scaffold has an AppBar with the title "Widget Tree Example.The body of the Scaffold contains a Center widget with a Column.In the Column, there's a Text widget displaying "Lvl 1: Stateless Widget" and a SizedBox.Another widget, MyStatefulWidget, is included in the Column.
MyStatefulWidget is a stateful widget that extends StatefulWidget.It has a state class _MyStatefulWidgetState. _MyStatefulWidgetState is the state class that extends State.It contains a counter variable _counter and a method _incrementCounter to increment the counter using setState.
The build method returns a Container with padding, a blue border, and a Column. In the Column, there's a Text widget displaying "Lvl 2: Stateful Widget" and a SizedBox. Another widget, CounterWidget, is included, passing the current counter value.
CounterWidget is a stateless widget that takes a counter parameter in its constructor.The build method returns a Container with padding, a green border, and a Column.In the Column, there's a Text widget displaying "Lvl 3: Stateless Widget" and a SizedBox.Another Text widget displays the counter value.

Level 1: MyApp2 - A stateless widget with a Scaffold containing an AppBar and a Column.
Level 2: MyStatefulWidget - A stateful widget managing a counter and displaying a child widget (CounterWidget).
Level 3: CounterWidget - A stateless widget displaying the counter value.



