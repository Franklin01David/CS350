# CS350

Summarize the project and what problem it was solving.
The Thermostat Lab project focused on creating a smart thermostat prototype for SysTec, a company looking to enter the smart thermostat market. The project involved using a Raspberry Pi to interface with hardware components such as an AHT2 temperature sensor (I2C), status LEDs (GPIO), buttons (GPIO interrupts), an LCD display, and UART communication to simulate cloud connectivity. The problem it addressed was the need for an embedded, low-level system that could read environmental data, interact with users through a physical interface, and prepare for future cloud integration.

The reflection paper reviewed the project experience and deeper considerations regarding emerging system architectures and technologies for scaling the prototype into a production-ready smart thermostat.

What did you do particularly well?
I feel that I did particularly well in implementing a functional state machine that handled multiple states (off, heating, cooling) cleanly and reliably. I also successfully integrated various hardware peripherals (I2C, GPIO, UART) while keeping the code modular, readable, and easy to expand. Additionally, my hardware architecture comparison was thorough, justifying each platform against business requirements, which demonstrated an ability to align technical decisions with business needs.

Where could you improve?
One area where I could improve is in error handling and robustness. Although the system worked under normal conditions, I could have added more defensive programming to anticipate and gracefully handle sensor read failures, UART communication errors, or button debounce issues. In future projects, I would also like to spend more time optimizing power consumption and resource management.

What tools and/or resources are you adding to your support network?
Through this project, I added several tools and resources to my support network. These include deeper experience with the GPIOZero library for Python hardware interaction, the smbus2 library for I2C communication, and practical UART serial communication techniques. I also strengthened my use of GitHub for version control and documentation, which will help organize and showcase future projects professionally.

What skills from this project will be particularly transferable to other projects and/or course work?
Many skills from this project are highly transferable, including writing interface software to control hardware components, designing maintainable and modular code using a state machine pattern, and analyzing hardware architectures to match business and technical needs. Understanding how to structure communication between software and hardware through protocols like I2C and UART will also be invaluable for future embedded systems work.

How did you make this project maintainable, readable, and adaptable?
I made the project maintainable and readable by using clear, consistent naming conventions, detailed inline comments, and modular functions for each hardware component (e.g., separate methods for reading temperature, updating the LCD, managing LED indicators). I structured the code so that new states or peripherals could be added easily without disrupting existing functionality. I also created thorough state machine documentation to make the system logic easy to understand for future developers who may work on extending the prototype.

