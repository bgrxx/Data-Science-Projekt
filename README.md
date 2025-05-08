# Verkehrsanalysen mit Sensordaten in Kalifornien

Dieses Projekt untersucht den Einfluss von Unfällen und Umweltfaktoren (insbesondere Niederschlag) auf die Dynamik des Verkehrsflusses in Kalifornien. Anhand von Echtzeitdaten des California Performance Measurement System (PeMS) aus dem Zeitraum Januar bis Dezember 2023 werden statistische Tests und Regressionsmodelle eingesetzt, um Muster und Zusammenhänge aufzudecken.

## Datenquellen

- **incidents.csv**: 476 766 Verkehrsvorfälle mit Angaben zu Ort, Dauer und Typ  
- **sensor_meta_feature.csv**: Metadaten zu 16 972 Sensorstandorten (Position, Infrastruktur, HOV-Spuren)  
- **p01_done.npy … p12_done.npy**: Fünf-Minuten-Messungen von Fahrzeugzahl, Belegung und Geschwindigkeit  
- **node_order.npy**: Mapping von Zeitreihen zu Sensor-IDs  

## Methodik

1. **Datenbereinigung**: Entfernen fehlerhafter Einträge, Zusammenführung doppelter Vorfälle, Imputation fehlender Sensorattribute  
2. **Hypothesentests**:  
   - Verkehrsfluss auf HOV-Spuren vor/nach Unfällen  

3. **Effektstärken**: Cliff’s Delta zur Quantifizierung praktischer Relevanz  

## Wichtige Ergebnisse

- **Geringfügige Änderungen** des Verkehrsflusses auf HOV-Spuren nach Unfällen (p < 0,0002; δ ≈ 0) , jedoch keine praktische Relevanz wegen Cliffs Delta

## Projektstruktur


