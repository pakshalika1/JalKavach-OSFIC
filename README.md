# JalKavach-OSFIC
JalKavach: Hyper-Local Flood &amp; Cyclone Early Warning System
Submission for the Odisha Seva First Innovation Challenge (OSFIC)
Target Area: Ganjam District, Odisha

THE PROBLEM
Coastal regions like Ganjam face severe, recurring threats from cyclonic storms, storm surges, and riverine flooding (e.g., Rushikulya river). Current warning systems often lack hyperlocal precision (village/ward level) and fail to integrate real-time, ground-level qualitative data (like citizen reports) with quantitative meteorological data, leading to delayed or generalized emergency responses.

THE SOLUTION
JalKavach is an offline-first, multimodal AI disaster intelligence dashboard. It fuses quantitative data (simulated river sensors, IMD cyclone tracks) with qualitative citizen reports to predict localized flood impacts. It provides actionable risk alerts, maps vulnerable locations, and calculates safe evacuation routes for emergency response forces (NDRF/ODRAF) and local citizens.

KEY FEATURES

Dynamic GIS Mapping and Risk Heatmaps: An interactive, offline-capable map of Ganjam showing low-lying inundation zones, simulated cyclone tracks, and real-time Village Risk Scores (0-100).

Smart Evacuation Routing: The system automatically calculates the safest paths from vulnerable villages to designated Cyclone Shelters (e.g., Gopalpur, Chhatrapur) while explicitly highlighting and avoiding roads blocked by floods or storm surges.

Citizen-in-the-Loop Reporting: An integrated UI to process crowd-sourced photos and texts. It uses on-device, regex-based analysis and image processing to estimate water depths and categorize hazards (e.g., power line hazard, rescue needed) without needing a backend connection.

Offline-First and SOS Integration: Built for zero-connectivity scenarios. Users can draft SOS messages containing their exact GPS coordinates, which are queued and sent via standard SMS the moment a cellular signal is detected.

OSDMA Live Telecast: A dedicated module to stream live emergency broadcasts and official bulletins from the Odisha State Disaster Management Authority.

AI Advisory Chatbot: An integrated conversational agent providing instant, context-aware safety protocols, evacuation guidance, and hazard reporting instructions.

TECHNOLOGY STACK
This repository contains the high-fidelity interactive frontend prototype of the Command Dashboard. For easy understanding and use, all the technology, UI, styling, and JavaScript logic used for this prototype have been put into a single HTML file. It uses embedded mock data to simulate real-time IoT feeds and AI routing.

Frontend UI: HTML5, CSS3, Vanilla JavaScript

Architecture: HTML Single-file Zero-Dependency Prototype (PWA foundations)

Mapping Engine: Custom SVG-based coordinate plotting and graph-based pathfinding (Dijkstra's algorithm adaptation).

Data Analysis: On-device Canvas API image analysis and regex natural language parsing.
