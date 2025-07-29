The balancing robot is controlled using an ESP 32.

Project in the simulator Wokwi can be found below:
[https://wokwi.com/projects/424801262978532353](https://wokwi.com/projects/436708660174793729)

<img width="980" height="790" alt="image" src="https://github.com/user-attachments/assets/1baf4d4a-61ce-4913-9eb8-e874c0026381" />

In this project the relay is used to control how many step motors are controlled at once from one port.  Either both are controlled by a port, or both can be individually controlled by their corresponding port.
Using the relay to connect both of the step motors to one port allows us to control both of them in sync.

The Rot function takes in the number of steps, n, the delay between each step, d, and the status of the motor/s, s.
The variable s, the status, let's us pick what the motors will do.  For example, when s is 3, the right step motor will rotate a wheel to go in the forward direction.
The lower the delay, d, the faster the motor/s complete the given number of steps, n, with status s.
