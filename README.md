# 🖥️ Monitoring Demo: Prometheus + Grafana + Docker

Projekt testowy stworzony w celu zademonstrowania umiejętności konfiguracji środowiska monitoringu serwera z wykorzystaniem narzędzi DevOps: Prometheus, Grafana, Docker.


## 📌 Technologie

- **Docker & Docker Compose**
- **Prometheus** – zbieranie metryk systemowych
- **Grafana** – wizualizacja danych z Prometheusa
- **Node Exporter** – eksport metryk z hosta
- **Linux / WSL** – środowisko uruchomieniowe

---

## ⚙️ Uruchomienie projektu

### 1. Klonuj repozytorium

```bash
git clone https://github.com/<twoja-nazwa-uzytkownika>/monitoring-demo.git
cd monitoring-demo
2. Uruchom kontenery
bash
Kopiuj
Edytuj
docker-compose up -d
Spowoduje to uruchomienie trzech kontenerów:

prometheus – nasłuchuje na localhost:9090

grafana – dostępna pod localhost:3000

node-exporter – zbiera metryki systemowe

🔍 Dostęp do aplikacji
Narzędzie	Adres URL	Login	Hasło
Prometheus	http://localhost:9090	—	—
Grafana	http://localhost:3000	admin	admin

📊 Screenshoty
Poniżej przykładowe widoki z uruchomionego środowiska:

Prometheus Targets	Grafana Dashboard

📁 Struktura katalogu
bash
Kopiuj
Edytuj
monitoring-demo/
├── docker-compose.yml
├── prometheus.yml
├── grafana/
│   └── (opcjonalnie provisioning/dashboards)
├── screens/
│   ├── grafana.png
│   └── prometheus.png
└── README.md
✍️ Autor
Projekt testowy wykonany przez Oskara Pozorskiego w ramach przygotowań do roli Junior DevOps Engineer.