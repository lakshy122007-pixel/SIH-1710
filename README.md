# Smart India Hackathon Workshop
# Date: 18/09/2026
## Register Number: 212225240076
## Name: Lakshiya Rajkumar

## Problem Title
SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations
## Problem Description
Background: Railway stations are complex environments with numerous facilities and locations such as ticket counters, platforms, restrooms, food courts, and waiting areas. Passengers often face difficulties in navigating these spaces, especially in large or unfamiliar stations. Efficient and user-friendly navigation systems are crucial for improving passenger experience, reducing congestion, and ensuring timely travel connections. Description: The problem involves developing a comprehensive navigation solution for railway stations that assists passengers in locating various facilities and destinations within the station premises. This includes creating detailed maps, providing real-time directions, and integrating features such as accessibility options for individuals with disabilities. The solution should be intuitive, easy to use, and accessible via multiple platforms, including mobile devices and digital kiosks. Key challenges include updating navigation information in real-time, ensuring accuracy, and accommodating the diverse needs of all passengers. Expected Solution: The expected solution is a multi-platform navigation system that provides detailed, real-time directions to all facilities and locations within a railway station. This system should include: A mobile application with 3D interactive maps and step-by-step navigation. Digital kiosks located throughout the station with touch-screen interfaces. Voice-guided navigation for visually impaired passengers. Regular updates to reflect changes in station layout and facility locations. Integration with existing railway apps and services for seamless user experience. The solution should enhance the overall passenger experience by reducing confusion, saving time, and improving accessibility within the station.

## Problem Creater's Organization
Ministry of Railway

## Idea
Idea : “RailWayFinder”
A station-level indoor navigation system that works like Google Maps, but inside a railway station.
Instead of only showing a map, the system understands the passenger's starting point, destination, preferred route and accessibility needs.
It can also guide passengers to toilets, ticket counters, food stalls, waiting rooms, drinking water, lifts, escalators, exits and parking areas.
The important part: the route is based on the actual station layout, not road maps.


## Proposed Solution / Architecture Diagram

1. Interactive Station Map

A digital map of the station showing:

-Platforms

-Ticket counters

-Foot-over bridges / subways

-Lifts & escalators

-Restrooms

-Food areas

-Waiting halls

-Enquiry counters

-Entrances/exits

-Parking areas

Users can simply select:
“Where I am” → “Where I want to go”
and receive a route.

2. Step-by-Step Indoor Navigation

Instead of giving only a line on a map, give instructions people can actually follow:
Walk straight for 40 m → Turn left → Take Lift 2 → Go to Level 1 → Platform 6 is on your right.
This makes it much more useful for first-time passengers.

3. Route Based on Passenger Needs

Before navigation, passengers can select:

- Normal route
  
- Wheelchair-friendly
  
- Luggage-friendly
  
- Fewer stairs
  
- Voice guidance

The system then removes unsuitable paths.

4. Station Change Updates

Station layouts can change because of:

-Platform changes
-Closed entrances
-Maintenance
-Lift/escalator outages
-Temporary barricades
-Construction

Instead of manually rebuilding the application, station authorities can update the affected location in the admin panel.
The navigation engine then avoids that path.

5. Mobile + Kiosk

The same navigation system can work through:
Mobile App/Web App
and
Station Touchscreen Kiosk

A passenger who doesn't have internet/mobile access can use a kiosk near the entrance.

## Use Cases

| User                           | Use Case                                |
| -------------------------------| --------------------------------------- |
|  First-time passenger          | Find platform without getting confused  |
|  Passenger with luggage        | Get a route with fewer stairs           |
|  Wheelchair user               | Find accessible routes, lifts and ramps |
|  Elderly passenger             | Choose a route with minimum walking     |
|  Visually impaired passenger   | Get voice-based directions              |
|  Passenger in a hurry          | Find the shortest route to the platform |
|  Passenger                     | Locate food court/restroom/waiting area |
|  Station staff                 | Update closed/changed facilities        |
|  Railway authority             | Monitor and maintain station map data   |


## Technology Stack
```
              RAILWAY NAVIGATION SYSTEM
                          │
        ┌─────────────────┼─────────────────┐
        ↓                 ↓                 ↓
    FRONTEND           BACKEND           DATABASE
   React / Next.js    Node.js + Express   PostgreSQL
        │                 │                 │
        └─────────────────┼─────────────────┘
                          ↓
                     MAP & ROUTING
                MapLibre / Mapbox
                     A* / Dijkstra
                          │
             ┌────────────┴────────────┐
             ↓                         ↓
         ACCESSIBILITY               UPDATES
       Web Speech API              Admin Panel
       Voice Guidance          Facility/Route Status
```   
## Dependencies
─ React / Next.js

─ Node.js + Express

─ PostgreSQL

─ MapLibre / Mapbox

─ A* / Dijkstra

─ Web Speech API

─ Git + GitHub
