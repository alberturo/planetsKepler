# 🌍 Kepler Habitable Planets Filter

This Node.js script parses NASA Kepler mission data (in CSV format) to identify potentially habitable exoplanets based on specific criteria. It uses the `csv-parse` library to process the data and filters planets based on size, temperature, and confirmation status.

## 📁 Project Structure

- `kepler_data.csv` – CSV file containing planetary data (must be present in the root folder).
- `index.js` – Main script that reads, parses, and filters the data.

## ✅ Habitable Planet Criteria

A planet is considered **habitable** if it meets **all** the following:

- **Disposition**: `koi_disposition` is `'CONFIRMED'`
- **Insolation Flux**: `koi_insol` is between `0.36` and `1.11` (Earth-like solar energy)
- **Planet Radius**: `koi_prad` is less than `1.6` Earth radii (likely rocky)

## ▶️ Usage

### 1. Install dependencies

```bash
npm install csv-parse
```
