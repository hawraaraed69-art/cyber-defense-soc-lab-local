# Cyber Defense SOC Lab (Local Edition)

A local-only cybersecurity operations lab built with **Streamlit** (`lab2.py`) and a local **FastAPI** agent (`local_agent.py`) running on `127.0.0.1:8000`, integrated with **Nmap**, **TShark/Wireshark**, and custom risk assessment modules in `core/`.

## Project Structure

```text
├── core/
│   ├── __init__.py
│   ├── nmap_scanner.py
│   ├── risk_assessment.py
│   └── traffic_analyzer.py
├── lab2.py
├── local_agent.py
└── requirements.txt
```

## Prerequisites

1. **Python** (3.10+ recommended)
2. **Nmap** (and **Npcap** on Windows) installed and added to system `PATH`
3. **Wireshark / TShark** installed and added to system `PATH`

## Installation & Setup

```bash
pip install -r requirements.txt
```

## Running the Lab Locally

Open **two** terminal windows inside the project directory:

1. **Start the Local Agent (Backend):**
   ```bash
   python local_agent.py
   ```

2. **Start the SOC Lab Dashboard (Frontend):**
   ```bash
   streamlit run lab2.py
   ```

## Usage Note

Use this lab strictly for educational purposes and on systems/networks you own or have explicit authorization to test.
