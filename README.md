# Drone Mission Planner

## What it does
A web app for drone operators to plan autonomous survey missions.
The operator draws a polygon over an area of interest on a map,
sets altitude and image overlap parameters, and the app generates
a lawnmower-pattern waypoint path covering the polygon. The app
displays estimated flight time, total distance, and waypoint count,
and exports the plan as GeoJSON or a MAVLink-compatible waypoint file.

## User stories
- As a mission operator, I can draw a survey polygon on a map so that I can define my area of interest without leaving the browser.
- As a mission operator, I can set altitude and overlap parameters so that the generated flight plan matches my sensor and coverage requirements.
- As a mission operator, I can export the generated waypoint plan as GeoJSON or MAVLink so that I can load it into my flight controller.

## Stack
- Frontend: React, TypeScript, Mapbox GL JS, Mapbox GL Draw
- Backend: FastAPI, Shapely
- Deployment: Vercel (frontend), Fly.io (backend)

## Milestone 1 (4 weeks)
User draws a polygon, sets altitude and overlap, sees a rendered
lawnmower waypoint path with flight time and distance estimates,
and exports GeoJSON. No auth, no database, no AWS.

## Status
In development
