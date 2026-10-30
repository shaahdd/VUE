🐔 Chicken Health Monitoring – Backend Learning Roadmap

🎯 Project Goal

Build a backend system that receives temperature, humidity, and ammonia readings from a Raspberry Pi, processes the data, stores readings, sends alerts, and updates a live dashboard.

🧰 Technologies

- C#
- ASP.NET Core Web API
- MQTT / MQTTnet
- SignalR
- SQL Server
- Entity Framework Core
- Twilio SMS
- Git & GitHub

---

Week 1 – C# Revision & ASP.NET Core Fundamentals

Weekly Summary

This week focuses on revising the C# fundamentals needed for the project, understanding how backend applications communicate over the internet, and learning how to build a basic ASP.NET Core Web API.

By the end of this week, you should be able to:

- Understand and write basic C# code.
- Work with classes, objects, collections, and JSON.
- Understand HTTP requests and responses.
- Create an ASP.NET Core Web API.
- Receive sensor readings through an API endpoint.

Day 1 – C# Fundamentals Revision

- [ ] "Variables, Data Types & Operators" (https://www.w3schools.com/cs/cs_variables.php)
- [ ] "Conditions – If, Else & Switch" (https://www.w3schools.com/cs/cs_conditions.php)
- [ ] "Loops – For, While & Foreach" (https://www.w3schools.com/cs/cs_loops.php)
- [ ] "Methods" (https://www.w3schools.com/cs/cs_methods.php)

Practice:

- Create a Console Application.
- Read temperature, humidity, and ammonia values.
- Check whether the temperature is within the normal range.
- Print an alert if a reading is critical.

Day 2 – OOP in C#

- [ ] "Classes and Objects" (https://www.w3schools.com/cs/cs_classes.php)
- [ ] "Constructors" (https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/constructors)
- [ ] "Properties" (https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/properties)
- [ ] "Inheritance" (https://www.w3schools.com/cs/cs_inheritance.php)
- [ ] "Interfaces" (https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/types/interfaces)

Practice:

- Create a "SensorReading" class.
- Add properties for Temperature, Humidity, and Ammonia.
- Create objects representing different sensor readings.

Day 3 – Collections, Exceptions & JSON

- [ ] "List and Dictionary" (https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/types/collections)
- [ ] "Exception Handling – Try & Catch" (https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/exceptions/exception-handling)
- [ ] "LINQ Basics" (https://learn.microsoft.com/en-us/dotnet/csharp/linq/)
- [ ] "JSON Serialization & Deserialization" (https://learn.microsoft.com/en-us/dotnet/standard/serialization/system-text-json/overview)

Practice:

- Store multiple sensor readings in a List.
- Use a Dictionary to store the latest reading for each box.
- Serialize a sensor reading to JSON.
- Deserialize JSON back into a C# object.

Day 4 – Networking Fundamentals

- [ ] "What is a Computer Network?" (https://www.cloudflare.com/learning/network-layer/what-is-a-computer-network/)
- [ ] "IP Addresses" (https://www.cloudflare.com/learning/network-layer/what-is-an-ip-address/)
- [ ] "Ports" (https://www.cloudflare.com/learning/network-layer/what-is-a-computer-port/)
- [ ] "TCP vs UDP" (https://www.cloudflare.com/learning/ddos/glossary/user-datagram-protocol-udp/)
- [ ] "HTTP and HTTPS" (https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview)

Practice:

- Understand how Raspberry Pi and backend server communicate.
- Understand the difference between an IP address and a port.
- Understand the request/response cycle.

Day 5 – ASP.NET Core Introduction

- [ ] "Introduction to ASP.NET Core" (https://learn.microsoft.com/en-us/aspnet/core/introduction-to-aspnet-core)
- [ ] "Create Your First Web API" (https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api)
- [ ] "Controllers and Actions" (https://learn.microsoft.com/en-us/aspnet/core/mvc/controllers/actions)
- [ ] "Dependency Injection" (https://learn.microsoft.com/en-us/dotnet/core/extensions/dependency-injection)
- [ ] "Middleware" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/middleware/)

Practice:

- Create an ASP.NET Core Web API project.
- Create a SensorController.
- Add a GET endpoint.
- Add a POST endpoint to receive sensor readings.

Day 6 – Async Programming & Configuration

- [ ] "Asynchronous Programming – Async and Await" (https://learn.microsoft.com/en-us/dotnet/csharp/asynchronous-programming/)
- [ ] "Task-Based Asynchronous Programming" (https://learn.microsoft.com/en-us/dotnet/standard/parallel-programming/task-based-asynchronous-programming)
- [ ] "Configuration in ASP.NET Core" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/configuration/)
- [ ] "Logging in .NET" (https://learn.microsoft.com/en-us/dotnet/core/extensions/logging)
- [ ] "Background Services" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/host/hosted-services)

Practice:

- Convert the API endpoints to async where appropriate.
- Add logging.
- Understand how background services work.

Day 7 – Week 1 Practical Application

Build: Basic Sensor API

- [ ] Create a "SensorReading" model.
- [ ] Create a "SensorController".
- [ ] Implement POST endpoint to receive readings.
- [ ] Implement GET endpoint to retrieve readings.
- [ ] Validate incoming sensor data.
- [ ] Test endpoints using Swagger or Postman.
- [ ] Push the project to GitHub.

Expected Result: A working API that can receive and return sensor readings.

---

Week 2 – MQTT, SignalR & SMS Notifications

Weekly Summary

This week focuses on communication between Raspberry Pi and the backend, real-time updates, and sending alerts when sensor readings exceed safe limits.

By the end of this week, you should be able to:

- Understand MQTT and its Publisher/Subscriber model.
- Receive sensor readings from an MQTT Broker using MQTTnet.
- Push live updates to connected clients using SignalR.
- Send SMS notifications using Twilio.
- Implement basic alert rules and avoid repeated notifications.

Day 8 – MQTT Fundamentals

- [ ] "What is MQTT?" (https://mqtt.org/)
- [ ] "MQTT Essentials" (https://www.hivemq.com/mqtt-essentials/)
- [ ] "MQTT Broker, Publisher & Subscriber" (https://www.hivemq.com/mqtt-essentials/)
- [ ] "MQTT Topics" (https://www.hivemq.com/mqtt-essentials/)
- [ ] "QoS Levels" (https://www.hivemq.com/mqtt-essentials/)

Practice:

- Install an MQTT Broker such as Mosquitto.
- Use an MQTT client to publish a test message.
- Subscribe to a topic and receive the message.
- Understand how the Raspberry Pi will publish sensor readings.

Day 9 – MQTT Advanced Concepts & MQTTnet

- [ ] "Retained Messages" (https://www.hivemq.com/mqtt-essentials/)
- [ ] "Last Will and Testament" (https://www.hivemq.com/mqtt-essentials/)
- [ ] "MQTTnet Documentation" (https://github.com/dotnet/MQTTnet)
- [ ] "MQTT Client Examples" (https://github.com/dotnet/MQTTnet)

Practice:

- Create an MQTT client in C#.
- Connect to the Broker.
- Subscribe to a sensor topic.
- Receive and deserialize JSON messages.

Day 10 – Integrating MQTT with ASP.NET Core

- [ ] "Hosted Services in ASP.NET Core" (https://learn.microsoft.com/en-us/aspnet/core/fundamentals/host/hosted-services)
- [ ] "Dependency Injection in .NET" (https://learn.microsoft.com/en-us/dotnet/core/extensions/dependency-injection)
- [ ] "JSON Serialization in .NET" (https://learn.microsoft.com/en-us/dotnet/standard/serialization/system-text-json/overview)

Practice:

- Create an "MqttService".
- Run the MQTT subscriber as a background service.
- Receive sensor messages.
- Validate and process incoming readings.
- Save readings or pass them to another service.

Day 11 – WebSocket & SignalR

- [ ] "What is WebSocket?" (https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API)
- [ ] "Introduction to SignalR" (https://learn.microsoft.com/en-us/aspnet/core/signalr/introduction)
- [ ] "SignalR Hubs" (https://learn.microsoft.com/en-us/aspnet/core/signalr/hubs)
- [ ] "SignalR JavaScript Client" (https://learn.microsoft.com/en-us/aspnet/core/signalr/javascript-client)

Practice:

- Create a "SensorHub".
- Send sensor updates from the backend through SignalR.
- Connect a simple client.
- Display new readings without refreshing the page.

Day 12 – Twilio SMS Integration

- [ ] "Twilio SMS Documentation" (https://www.twilio.com/docs/messaging)
- [ ] "Twilio C#/.NET Documentation" (https://www.twilio.com/docs/libraries/csharp-dotnet)
- [ ] "Twilio Quickstart" (https://www.twilio.com/docs/messaging/quickstart)

Practice:

- Create a Twilio account.
- Configure the required credentials securely.
- Send a test SMS from a C# application.
- Handle errors when sending messages.

Day 13 – Alert System

- [ ] Implement temperature thresholds.
- [ ] Implement humidity thresholds.
- [ ] Implement ammonia thresholds.
- [ ] Create an "AlertService".
- [ ] Send an SMS when a critical reading is received.
- [ ] Add a cooldown period to prevent repeated SMS messages.
- [ ] Log alerts and their timestamps.

Practice:

- Simulate sensor readings.
- Test normal and critical conditions.
- Verify that alerts are sent only when needed.

Day 14 – Week 2 Practical Application

Build: Real-Time Sensor Monitoring

- [ ] Connect the backend to an MQTT Broker.
- [ ] Receive sensor readings from MQTT.
- [ ] Deserialize and validate the readings.
- [ ] Send readings to SignalR clients.
- [ ] Implement alert thresholds.
- [ ] Send SMS notifications using Twilio.
- [ ] Test the complete communication flow.
- [ ] Push the project to GitHub.

Expected Result: The backend receives sensor readings through MQTT, updates connected clients in real time, and sends SMS alerts for critical readings.

---

Week 3 – Database, Authentication & Final Integration

Weekly Summary

This week focuses on storing sensor readings, managing database operations, securing the backend, and integrating all components into one working system.

By the end of this week, you should be able to:

- Understand SQL and relational databases.
- Use Entity Framework Core to communicate with the database.
- Store and retrieve sensor readings.
- Understand authentication and authorization.
- Protect API endpoints.
- Integrate all project components.

Day 15 – Database & SQL Fundamentals

- [ ] "What is a Database?" (https://www.oracle.com/database/what-is-database/)
- [ ] "SQL Introduction" (https://www.w3schools.com/sql/sql_intro.asp)
- [ ] "SQL SELECT" (https://www.w3schools.com/sql/sql_select.asp)
- [ ] "SQL INSERT" (https://www.w3schools.com/sql/sql_insert.asp)
- [ ] "SQL UPDATE & DELETE" (https://www.w3schools.com/sql/sql_update.asp)
- [ ] "Primary Keys & Foreign Keys" (https://www.w3schools.com/sql/sql_foreignkey.asp)

Practice:

- Create a database for the chicken health monitoring system.
- Create tables for Farms, Hangars, Boxes, SensorReadings, and Alerts.
- Insert and retrieve sample data.

Day 16 – Entity Framework Core

- [ ] "Introduction to Entity Framework Core" (https://learn.microsoft.com/en-us/ef/core/)
- [ ] "DbContext and DbSet" (https://learn.microsoft.com/en-us/ef/core/dbcontext-configuration/)
- [ ] "Relationships" (https://learn.microsoft.com/en-us/ef/core/modeling/relationships)
- [ ] "Migrations" (https://learn.microsoft.com/en-us/ef/core/managing-schemas/migrations/)
- [ ] "Querying Data with EF Core" (https://learn.microsoft.com/en-us/ef/core/querying/)

Practice:

- Install EF Core packages.
- Create "ApplicationDbContext".
- Create entity models.
- Configure relationships.
- Create and apply the first migration.

Day 17 – Saving & Retrieving Sensor Data

- [ ] Implement sensor readings repository or data service.
- [ ] Save incoming MQTT readings to the database.
- [ ] Retrieve readings by box number.
- [ ] Retrieve readings by date range.
- [ ] Retrieve the latest reading for each box.
- [ ] Add basic database indexes where useful.

Practice:

- Connect the MQTT service to the database.
- Verify that every valid reading is stored.
- Create API endpoints to retrieve historical readings.

Day 18 – Authentication & Authorization

- [ ] "Authentication and Authorization in ASP.NET Core" (https://learn.microsoft.com/en-us/aspnet/core/security/)
- [ ] "JWT Bearer Authentication" (https://learn.microsoft.com/en-us/aspnet/core/security/authentication/configure-jwt-bearer-authentication)
- [ ] "Claims-Based Authorization" (https://learn.microsoft.com/en-us/aspnet/core/security/authorization/claims)
- [ ] "Role-Based Authorization" (https://learn.microsoft.com/en-us/aspnet/core/security/authorization/roles)

Practice:

- Understand the difference between Authentication and Authorization.
- Protect selected API endpoints.
- Understand how roles can distinguish between Admin and Farm Manager.

Day 19 – Security, Testing & Error Handling

- [ ] "ASP.NET Core Security Best Practices" (https://learn.microsoft.com/en-us/aspnet/core/security/)
- [ ] "Unit Testing in .NET" (https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-with-dotnet-test)
- [ ] "Integration Tests in ASP.NET Core" (https://learn.microsoft.com/en-us/aspnet/core/test/integration-tests)
- [ ] "Secrets Management in .NET" (https://learn.microsoft.com/en-us/aspnet/core/security/app-secrets)

Practice:

- Store credentials using User Secrets or environment variables.
- Never commit passwords, API keys, or Twilio credentials.
- Test sensor validation and alert logic.
- Handle invalid data and service failures.
- Add useful logs.

Day 20 – Final Project Integration

Integrate all backend components:

- [ ] Raspberry Pi sends sensor readings.
- [ ] MQTT Broker receives published messages.
- [ ] ASP.NET Core MQTT service subscribes to topics.
- [ ] Backend validates incoming JSON.
- [ ] Sensor readings are stored in the database.
- [ ] SignalR broadcasts live updates.
- [ ] AlertService checks thresholds.
- [ ] Twilio sends SMS notifications.
- [ ] API endpoints provide historical readings.
- [ ] Authentication protects the required endpoints.

Day 21 – Final Testing & Documentation

- [ ] Test the complete system from sensor to backend.
- [ ] Test normal and critical sensor readings.
- [ ] Test MQTT disconnection and reconnection.
- [ ] Test database storage and retrieval.
- [ ] Test SignalR live updates.
- [ ] Test Twilio notifications.
- [ ] Fix bugs and improve error handling.
- [ ] Write the project README.
- [ ] Document API endpoints and MQTT topics.
- [ ] Upload the final project to GitHub.

Expected Result: A complete Chicken Health Monitoring Backend with MQTT communication, real-time updates, database storage, and SMS alerts.

---

🧪 Final Project Architecture

Raspberry Pi
     |
     | Sensor Readings (JSON)
     v
 MQTT Broker
     |
     v
 ASP.NET Core Backend
     |
     |---- MQTTnet Service
     |
     |---- Data Validation
     |
     |---- Alert Service
     |         |
     |         v
     |      Twilio SMS
     |
     |---- Entity Framework Core
     |         |
     |         v
     |       Database
     |
     v
  SignalR Hub
     |
     v
 Live Dashboard

⭐ Priority Guide

Must Learn

- C# Fundamentals & OOP
- Async/Await
- ASP.NET Core Web API
- HTTP & Networking Basics
- MQTT & MQTTnet
- SignalR
- JSON
- Twilio Integration

Important

- SQL
- Entity Framework Core
- Authentication & Authorization
- Dependency Injection
- Background Services
- Testing & Logging

Optional / Advanced

- Database Internals
- B-Trees and Storage Engines
- Advanced OAuth
- Advanced MQTT Performance Optimization

---

📌 Important Notes

- Focus on understanding and implementing, not just watching tutorials.
- Every day should end with working code.
- Use GitHub to track your progress.
- Don't spend too much time on advanced topics before completing the basic backend.
- The goal is to finish with a working integrated project, not just theoretical knowledge.
