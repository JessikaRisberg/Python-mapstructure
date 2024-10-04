# Soltak

Detta projekt utför beräkningar för olika kunder.

## Installation

1. Klona repositoryt:
    ```bash
    git clone <repo-url>
    cd my_project
    ```

2. Skapa och aktivera en virtuell miljö:
    ```bash
    python -m venv env
    source env/bin/activate  # På Windows använd: env\Scripts\activate
    ```

3. Installera beroenden:
    ```bash
    pip install -r requirements.txt
    ```

4. Skapa en `.env`-fil med dina API-nycklar:
    ```plaintext
    # Stenungsund
    STENUNGSUND_API_KEY=din_api_key_for_stenungsund
    # Tjörn
    TJORN_API_KEY=din_api_key_for_tjorn
    # Kungälv
    KUNGALV_API_KEY=din_api_key_for_kungalv
    ```

## Användning

För att köra beräkningarna:
```bash
python scripts/run_calculations.py
_____________________________________________________________________-

Structure of project
SOLTAK/
│
├── calculations/
│   ├── __init__.py
│   └── delta_calculations.py
│
├── config/
│   ├── __init__.py
│   ├── stenungsund_config.py
│   ├── tjorn_config.py
│   ├── kungalv_config.py
│   └── lynx_client.py
│
├── scripts/
│   ├── __init__.py
│   └── run_calculations.py
│
├── tests/
│   ├── __init__.py
│   ├── test_delta_calculations.py
│   └── test_lynx_client.py
│
├── .gitignore
├── README.md
├── requirements.txt
└── setup.py