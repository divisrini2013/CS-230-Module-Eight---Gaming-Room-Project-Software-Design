**# CS-230-Module-Eight---Gaming-Room-Project-Software-Design**

**Briefly summarize The Gaming Room client and their software requirements.**

The Gaming Room wants to create a modern, interactive game based on the 1980s drawing and guessing game Win, Lose or Draw. They want to make Draw It or Lose It, a web and Android game, fun and engaging for players on numerous devices. The customer wanted a solution that supports numerous players on various teams with real-time synchronization across desktop web browsers and Android mobile devices.
Having numerous teams with their own names and players and only one instance of the game operating at a time were key business needs. Allowing only one active gaming session ensures players participate without dispute. For wide accessibility, the game must enable a seamless user experience across devices. Technical needs included unique identities for each game, team, and player, concurrent user access, and fast player syncing during gameplay. The system has to be stable, expandable, and able to manage peak gaming demands.

**What did you do particularly well in developing this documentation?**

This documentation's clarity and complete covering of functional and non-functional requirements were its strengths. I successfully transformed the client's vision into a workable design blueprint. The detailed system architecture view and domain model helped developers and stakeholders understand how the game would be structured, how components (e.g., game, team, player) would interact, and how the Singleton pattern would enforce only one game instance at a time. A well-done concurrency management portion prevented data corruption and ensured data consistency across several participants.
I thoroughly assessed the development platforms' applicability for this project. My evaluation of macOS, Linux, Windows, and mobile devices' server-side hosting, client-side development tools, and license prices helped me choose the best platform for game creation and deployment. The development team knew which platform would fulfill the game's scalability, pricing, and technological needs.

**What about the process of working through a design document did you find helpful when developing the code?**

Working through the design document before writing code was quite beneficial because it gave a structured way to solving the problem. It made me evaluate the complete system, user experience, bottlenecks, and scalability issues in advance. I broke down the challenge into smaller, more manageable chunks by defining a clear system architecture and the behaviors and interactions of distinct entities (game, team, player). Knowing how each component should behave and interact with other system components made coding easier.
The design document also defined development expectations by describing technical constraints like concurrent users and real-time syncing. It helped me create state management and concurrency handling first before moving on to other features.

**If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?**

Scalability and fault tolerance would be my documentation revision. I covered microservices and distributed systems, however I could have expanded on scaling methods like load balancing, auto-scaling, and database sharding. WebSockets and RabbitMQ are used for real-time communication and background jobs, but I might have shown how they would be combined with a cloud-based architecture for high availability and fault tolerance. I would describe data replication, backup, and disaster recovery procedures to keep the system running smoothly even under tremendous loads or failure.

**How did you interpret the user’s needs and implement them into your software design?**

I examined The Gaming Room's requirements and identified essential elements that would improve gameplay to determine the user's wants. For real-time synchronization among numerous players, I recommended WebSocket connections for low-latency, bi-directional client-server communication. Knowing that people will play the game on numerous devices, I prioritized cross-platform compatibility to make sure it worked properly on desktop web browsers and Android mobile devices.
The client's requirement for many teams with unique names and players led to a solution that supports creating and managing game entities like teams, players, and games with unique identifiers. I made the system modular and flexible to allow future updates and features by using inheritance and polymorphism. The Singleton pattern achieved the requirement for one active game instance in memory, preventing conflicts and guaranteeing a consistent, seamless experience for all players.

**Why is it so important to consider the user’s needs when designing?**

Because software success depends on meeting user demands, user needs must be considered. A design that doesn't meet user expectations will frustrate users and fail to engage the intended audience. I designed an entertaining and functional system by knowing the client's gaming dynamics, user preferences, and technical needs. The system needed high concurrency and low-latency communication for fast-paced, real-time sketching and guessing, thus I recommended WebSockets and microservices.
Considering user demands ensures that software is accessible, dependable, and scalable. By considering diverse platforms and devices, I was able to build the game to run on desktop computers and mobile phones, improving the user experience and expanding the audience.

**How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?**

I designed software using object-oriented principles and design patterns. After splitting the system down into game, team, and player components, I used inheritance and encapsulation to represent their relationships. I used the Singleton technique to handle the game's state and ensure one instance ran at a time. I also picked a microservices architecture for scalability and fault tolerance to grow and respond to customer demand.
Later, I will utilize a similar strategy but prioritize user feedback during design. Based on real-world feedback from user interviews or usability testing, I would tweak the design to meet user expectations. I would also prioritize efficiency and security from the start, building the system to efficiently manage large numbers of users while protecting data.
