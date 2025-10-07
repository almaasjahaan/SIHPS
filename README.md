# Smart India Hackathon Workshop
# Date: 7/10/25
## Register Number:212224230016
## Name: Almaas Jahaan M
## Problem Title
SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations
## Problem Description
Background: Railway stations are complex environments with numerous facilities and locations such as ticket counters, platforms, restrooms, food courts, and waiting areas. Passengers often face difficulties in navigating these spaces, especially in large or unfamiliar stations. Efficient and user-friendly navigation systems are crucial for improving passenger experience, reducing congestion, and ensuring timely travel connections. Description: The problem involves developing a comprehensive navigation solution for railway stations that assists passengers in locating various facilities and destinations within the station premises. This includes creating detailed maps, providing real-time directions, and integrating features such as accessibility options for individuals with disabilities. The solution should be intuitive, easy to use, and accessible via multiple platforms, including mobile devices and digital kiosks. Key challenges include updating navigation information in real-time, ensuring accuracy, and accommodating the diverse needs of all passengers. Expected Solution: The expected solution is a multi-platform navigation system that provides detailed, real-time directions to all facilities and locations within a railway station. This system should include: A mobile application with 3D interactive maps and step-by-step navigation. Digital kiosks located throughout the station with touch-screen interfaces. Voice-guided navigation for visually impaired passengers. Regular updates to reflect changes in station layout and facility locations. Integration with existing railway apps and services for seamless user experience. The solution should enhance the overall passenger experience by reducing confusion, saving time, and improving accessibility within the station.

## Problem Creater's Organization
Ministry of Railway

## Idea
Electronic waste (e-waste) like mobiles, laptops, batteries, and appliances is often
discarded improperly, leading to soil/water pollution and health hazards. Many people
are unaware of where to dispose e-waste safely.
Our idea: A digital platform (web/mobile app) that helps citizens easily locate the
nearest certified e-waste facilities, schedule pickups, and raise awareness about proper
disposal.

## Proposed Solution / Architecture Diagram
## Workflow
1.User Access User enters location / shares GPS. Platform shows nearest certified ewaste collection centers on a map. Option to request pickup (home/office).

2.Backend Processing Facility data stored in a database. APIs handle search (by distance
& items accepted), pickup scheduling, and verification.

3.Facility/Admin Dashboard Facilities can approve/reject pickup requests. Upload
certifications, operating hours, and accepted items.

4.Optional Intelligence Layer Suggests optimal pickup routes. Provides analytics (e.g.,
total e-waste collected).

## Architecture Diagram
<img width="1305" height="801" alt="Screenshot 2025-10-07 151958" src="https://github.com/user-attachments/assets/be0adac7-e8a5-47b0-8617-f7c109628047" />


## Use Cases
1.Citizen / User Find nearest certified e-waste drop-off points. See what items are
accepted (phones, batteries, appliances). Schedule pickup from home/office. Get ecopoints/rewards for recycling.

2.Facility Operator Register facility with details, certifications, and items accepted.
Manage pickup requests. Update operational status/hours.

3.Admin (Govt/NGO) Verify facilities (certification check). Monitor total e-waste
collected. Analyze hotspots (areas generating most e-waste)

## Technology Stack
Frontend: React.js (with Leaflet.js for maps) Tailwind CSS (UI styling)

Backend: Node.js + Express (REST APIs) (or Flask/FastAPI if Python preferred)

Database: PostgreSQL (with PostGIS for geo queries) MongoDB (optional, for flexible
facility metadata)

Maps & Geolocation: OpenStreetMap + Leaflet.js

Authentication: Firebase Auth or Auth0 (quick hackathon integration)

Hosting: Frontend → Vercel/Netlify Backend → Render/Heroku/Railway Database → Supabase/Postgres Cloud

## Dependencies
Frontend react react-router-dom leaflet + react-leaflet tailwindcss

Backend express pg (Postgres client) cors, dotenv, jsonwebtoken (for auth/security)

Optional postgis extension (for geo queries) multer (for file uploads e.g., certificates)
socket.io (for real-time status updates)

