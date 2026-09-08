# SIH - Industrial Fire & Persistent Thermal Source Detection (PS 162)

An automated intelligence system fusing NASA FIRMS VIIRS/MODIS telemetry with OpenStreetMap infrastructure boundaries and spatial clustering to separate routine industrial flaring from acute fire disasters.

## Project Structure
- `src/ingest_firms.py`: Telemetry ingestion and preprocessing.
- `src/osm_polygons.py`: OSM industrial boundary extraction via Overpass API.
- `src/clustering.py`: Haversine DBSCAN spatial clustering and FRP baseline modeling.
- `src/classifier.py`: Hazard classification and feature importance.
- `dashboard/`: Interactive geospatial interface.

## Setup Instructions
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt