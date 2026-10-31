VUE — 21-Day Backend Roadmap

Project Goal

Build the backend of a chicken health monitoring system using C#, ASP.NET Core, SQL Server, MQTT, SignalR, and Twilio.

Duration: 21 Days · 3 Weeks
Daily Commitment: 2–4 Hours
Main Track: Backend Development with .NET

---

Week 1 — C# & ASP.NET Core Fundamentals

Goal: Build a REST API connected to SQL Server using Entity Framework Core.

Day 1 — OOP, Async & Exception Handling

Estimated Time: 3 Hours

- [ ] Revise OOP: Classes, Objects, Encapsulation, Inheritance, Polymorphism, Abstraction, and Interfaces.
- [ ] Write a small practical OOP exercise.
- [ ] Review Async/Await.
- [ ] Review Exception Handling.

Resources:

- "CodeGraphia — C# OOP" (https://www.youtube.com/playlist?list=PLX1bW_GeBRhAfq0EsDHH4YemBAd6G-H75)
- "Microsoft — Object-Oriented Programming" (https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/object-oriented/)

Day 2 — Collections & HTTP Basics

Estimated Time: 3.5 Hours

- [ ] Understand Collections and Generics.
- [ ] Practice List, Dictionary, HashSet, Stack, and Queue.
- [ ] Understand HTTP methods: GET, POST, PUT, DELETE.
- [ ] Understand HTTP Status Codes and JSON.
- [ ] Learn REST API principles.

Resources:

- "CodeGraphia — Advanced C#" (https://www.youtube.com/playlist?list=PLX1bW_GeBRhBbnebNayUDYlQJRBKwZKlo)
- "Microsoft — Collection Types" (https://learn.microsoft.com/en-us/dotnet/standard/collections/commonly-used-collection-types)
- "MDN — HTTP Overview" (https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview)

Day 3 — ASP.NET Core Introduction

Estimated Time: 3.5 Hours

- [ ] Understand ASP.NET Core project structure.
- [ ] Learn Controllers and Routing.
- [ ] Understand Dependency Injection.
- [ ] Create your first Web API.
- [ ] Test a basic endpoint.

Resources:

- "CodeGraphia — ASP.NET Core" (https://www.youtube.com/playlist?list=PLX1bW_GeBRhAjpkPCTpKXJoFGe2ZpYGUC)
- "Microsoft — First Web API" (https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api)
- "Microsoft — Dependency Injection" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection)

Day 4 — SQL & LINQ Basics

Estimated Time: 3.5 Hours

- [ ] Review relational databases.
- [ ] Understand Tables, Primary Keys, and Foreign Keys.
- [ ] Practice SELECT, INSERT, UPDATE, and DELETE.
- [ ] Understand basic JOIN operations.
- [ ] Learn LINQ basics: IEnumerable, Lambda, Where, Select, and OrderBy.

Resources:

- "Database Fundamentals Video" (https://youtu.be/pPqazMTzNOM)
- "SQLBolt — Interactive SQL Lessons" (https://sqlbolt.com/)
- "Ahmed Mohamady — LINQ in C#" (https://eg-24.com/courses/كورس-لغة-الإستعلامات-linq-مع-c/)
- "Microsoft — LINQ" (https://learn.microsoft.com/en-us/dotnet/csharp/linq/)

Day 5 — Entity Framework Core

Estimated Time: 3.5 Hours

- [ ] Understand ORM and EF Core.
- [ ] Learn DbContext and DbSet.
- [ ] Create Models.
- [ ] Practice Migrations.
- [ ] Connect ASP.NET Core to SQL Server.

Resources:

- "Microsoft — EF Core Getting Started" (https://learn.microsoft.com/en-us/ef/core/get-started/)
- "EF Core SQL Server Provider" (https://learn.microsoft.com/en-us/ef/core/providers/sql-server/)
- "EF Core Migrations" (https://learn.microsoft.com/en-us/ef/core/managing-schemas/migrations/)

Day 6 — Advanced LINQ & Database Design

Estimated Time: 3.5 Hours

- [ ] Practice First, Single, Any, and All.
- [ ] Learn GroupBy, Join, and Aggregation.
- [ ] Understand Deferred and Immediate Execution.
- [ ] Design the SensorReadings table.
- [ ] Design the Devices table.
- [ ] Design the Alerts table.
- [ ] Define relationships between tables.

Resources:

- "Microsoft — LINQ Query Walkthrough" (https://learn.microsoft.com/en-us/dotnet/csharp/linq/get-started/walkthrough-writing-queries-linq)
- "dbdiagram — Relationships" (https://docs.dbdiagram.io/relationships/)

Day 7 — Week 1 Practical Task

Estimated Time: 4 Hours

- [ ] Create an ASP.NET Core Web API.
- [ ] Connect it to SQL Server using EF Core.
- [ ] Implement CRUD operations for SensorReadings.
- [ ] Test endpoints using Postman.
- [ ] Review the week's topics and fix any issues.

Resources:

- "Postman — Quick Start" (https://learning.postman.com/docs/getting-started/quick-start/)
- "Microsoft — First Web API" (https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api)

Week 1 Deliverable: A working REST API connected to SQL Server.

---

Week 2 — MQTT & Real-Time Data

Goal: Receive sensor data through MQTT, process it in the backend, and display updates in real time.

Day 8 — MQTT Fundamentals

Estimated Time: 3 Hours

- [ ] Understand MQTT architecture.
- [ ] Learn Publisher and Subscriber.
- [ ] Understand Broker, Topics, and Payloads.
- [ ] Learn QoS levels.

Resources:

- "MQTT Introduction Video" (https://youtu.be/l_CT1sGgvdk)
- "HiveMQ — MQTT Essentials" (https://www.hivemq.com/blog/mqtt-essentials-part-1-introducing-mqtt/)

Day 9 — MQTT Broker

Estimated Time: 3.5 Hours

- [ ] Understand MQTT Broker responsibilities.
- [ ] Install Mosquitto.
- [ ] Publish test messages.
- [ ] Subscribe to MQTT topics.
- [ ] Test communication between publisher and subscriber.

Resources:

- "Mosquitto Documentation" (https://mosquitto.org/documentation/)
- "Mosquitto Manual" (https://mosquitto.org/man/)

Day 10 — MQTTnet

Estimated Time: 3.5 Hours

- [ ] Install MQTTnet in the ASP.NET Core project.
- [ ] Create an MQTT client.
- [ ] Connect to the Broker.
- [ ] Subscribe to sensor topics.
- [ ] Receive incoming messages.

Resources:

- "MQTTnet GitHub" (https://github.com/dotnet/MQTTnet)
- "MQTTnet Samples" (https://github.com/dotnet/MQTTnet/tree/master/Samples)

Day 11 — Background Services

Estimated Time: 3.5 Hours

- [ ] Understand BackgroundService.
- [ ] Learn IHostedService.
- [ ] Run MQTT subscription as a background service.
- [ ] Handle connection and disconnection.
- [ ] Test the service while the application is running.

Resources:

- "Microsoft — Hosted Services" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/host/hosted-services)

Day 12 — Process & Store Sensor Data

Estimated Time: 4 Hours

- [ ] Define the sensor JSON payload.
- [ ] Deserialize incoming MQTT messages.
- [ ] Validate temperature, humidity, and ammonia values.
- [ ] Save valid readings to SQL Server.
- [ ] Handle invalid messages and errors.
- [ ] Test the complete data-processing flow.

Resources:

- "Microsoft — JSON Deserialization" (https://learn.microsoft.com/en-us/dotnet/standard/serialization/system-text-json/deserialization)
- "ASP.NET Core — Model Validation" (https://learn.microsoft.com/en-us/aspnet/core/mvc/models/validation)

Day 13 — SignalR

Estimated Time: 3.5 Hours

- [ ] Understand WebSockets and SignalR.
- [ ] Create a SignalR Hub.
- [ ] Send sensor updates to connected clients.
- [ ] Test real-time communication.

Resources:

- "Microsoft — SignalR Introduction" (https://learn.microsoft.com/en-us/aspnet/core/signalr/introduction)
- "Microsoft — SignalR Hubs" (https://learn.microsoft.com/en-us/aspnet/core/signalr/hubs)

Day 14 — Week 2 Integration Task

Estimated Time: 4 Hours

- [ ] Receive MQTT messages.
- [ ] Process and validate sensor data.
- [ ] Store readings in SQL Server.
- [ ] Broadcast updates using SignalR.
- [ ] Test the full flow.

Week 2 Deliverable: A working real-time sensor data pipeline.

---

Week 3 — Authentication, Alerts & Final Integration

Goal: Add authentication, alert notifications, testing, and complete the backend integration.

Day 15 — Authentication & Authorization

Estimated Time: 4 Hours

- [ ] Understand Authentication vs Authorization.
- [ ] Learn ASP.NET Core Identity basics.
- [ ] Understand JWT Authentication.
- [ ] Learn Role-Based Authorization.
- [ ] Protect API endpoints.

Resources:

- "Authentication & Authorization Playlist" (https://www.youtube.com/playlist?list=PLOeFnOV9YBa4yaz-uIiT5ZW3QQGHJQXi)
- "Microsoft — ASP.NET Core Authentication" (https://learn.microsoft.com/en-us/aspnet/core/security/authentication/)
- "Microsoft — ASP.NET Core Identity" (https://learn.microsoft.com/en-us/aspnet/core/security/authentication/identity)
- "Microsoft — JWT Bearer Authentication" (https://learn.microsoft.com/en-us/aspnet/core/security/authentication/configure-jwt-bearer-authentication)

Day 16 — Twilio SMS

Estimated Time: 3 Hours

- [ ] Understand Twilio SMS API.
- [ ] Create a Twilio account.
- [ ] Configure credentials securely.
- [ ] Send a test SMS from ASP.NET Core.

Resources:

- "Twilio — SMS Quickstart (C# / .NET Core)" (https://www.twilio.com/docs/messaging/quickstart/csharp-dotnet-core)

Day 17 — Alert Logic

Estimated Time: 4 Hours

- [ ] Define safe ranges for temperature, humidity, and ammonia.
- [ ] Detect abnormal readings.
- [ ] Create alert records in SQL Server.
- [ ] Send SMS notifications when thresholds are exceeded.
- [ ] Prevent repeated unnecessary notifications.
- [ ] Test different alert scenarios.

Resources:

- "EF Core Documentation" (https://learn.microsoft.com/en-us/ef/core/)
- "Twilio Messaging Documentation" (https://www.twilio.com/docs/messaging)

Day 18 — Security & Configuration

Estimated Time: 3.5 Hours

- [ ] Use appsettings and environment variables.
- [ ] Keep secrets out of source control.
- [ ] Validate incoming data.
- [ ] Handle exceptions and logging.
- [ ] Secure API endpoints.

Resources:

- "Microsoft — ASP.NET Core Configuration" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/configuration/)
- "Microsoft — Secret Manager" (https://learn.microsoft.com/en-us/aspnet/core/security/app-secrets)
- "Microsoft — Logging" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/logging/)

Day 19 — Testing

Estimated Time: 4 Hours

- [ ] Test API endpoints using Postman.
- [ ] Test MQTT message handling.
- [ ] Test database operations.
- [ ] Test SignalR updates.
- [ ] Test SMS alert scenarios.
- [ ] Fix discovered issues.

Resources:

- "Postman — Test Scripts" (https://learning.postman.com/docs/tests-and-scripts/write-scripts/test-scripts/)
- "Microsoft — ASP.NET Core Integration Tests" (https://learn.microsoft.com/en-us/aspnet/core/test/integration-tests)

Day 20 — Full System Integration

Estimated Time: 4 Hours

- [ ] Connect Raspberry Pi or a simulated sensor publisher.
- [ ] Connect MQTT Broker.
- [ ] Receive messages through MQTTnet.
- [ ] Store readings using EF Core.
- [ ] Broadcast updates using SignalR.
- [ ] Trigger alerts through Twilio.
- [ ] Test the complete end-to-end workflow.

Deliverable: Complete end-to-end backend workflow.

Day 21 — Final Review

Estimated Time: 3–4 Hours

- [ ] Review project architecture.
- [ ] Fix bugs and improve error handling.
- [ ] Organize the project structure.
- [ ] Write README documentation.
- [ ] Add an architecture diagram.
- [ ] Test the complete workflow.
- [ ] Review what was learned and identify remaining gaps.

Week 3 Deliverable: Complete backend integration with real-time monitoring and SMS alerts.

---

System Architecture

Raspberry Pi Sensors
↓
MQTT Broker
↓
MQTTnet Subscriber
↓
Data Validation
↓
SQL Server
├── SignalR → Dashboard
└── Alert Service → Twilio SMS

---

Final Project Checklist

- [ ] ASP.NET Core Web API
- [ ] SQL Server Database
- [ ] Entity Framework Core
- [ ] MQTT Broker
- [ ] MQTTnet Subscriber
- [ ] Background Service
- [ ] Sensor Data Validation
- [ ] SignalR Real-Time Updates
- [ ] Authentication & Authorization
- [ ] Twilio SMS Notifications
- [ ] Testing & Documentation

---

Important: Don't just watch tutorials. Write code, test each feature, and make sure you understand how the components work together.
