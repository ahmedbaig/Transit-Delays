# transit-delays

Transport for NSW real-time feeds into PostGIS, with a model predicting delays across the Sydney network.

## Phases

1. **Feeds:** GTFS static timetable plus GTFS-realtime trip updates and vehicle positions, polled continuously.
2. **Storage:** a PostGIS schema for stops, routes, shapes, positions and observed delays, with retention rules.
3. **Model:** a historical baseline, then a model using time, route, location and events.
4. **Viewer:** a live delay map on the geo platform.
