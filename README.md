# Hoja de Trabajo 6 – Modelación y Simulación

Repositorio de la Hoja de Trabajo 6 (CC2017, grupo 5). Contiene un notebook por cada task:

- **Task 1** (`Task1.ipynb`): análisis analítico de un modelo de Lotka-Volterra competitivo entre dos plataformas, con los parámetros del grupo 5 (equilibrios, jacobiana y clasificación, nulclinas y campo vectorial).
- **Task 2** (`Task2.ipynb`): simulación numérica del mismo modelo con Euler y RK4 propios, retrato de fases, cuencas de atracción, estabilidad local, paso máximo de Euler e intervenciones.
- **Task 3** (`Task3.ipynb`): modelo de un lago con reciclaje de nutrientes, ẋ = a − b·x + x²/(x²+1) con b = 0.55. Incluye el diagrama de equilibrios y la histéresis con un barrido lento de la carga, y las señales de alerta temprana (varianza y autocorrelación con Euler-Maruyama propio, detrending, ventanas móviles y tau de Kendall, con el control de falsas alarmas).

Las figuras generadas se guardan en `img/`.

## Cómo levantarlo

Se recomienda Python 3.10+ (probado con 3.14).

Windows (PowerShell):

```powershell
git clone https://github.com/jruiz002/task1_ms.git
cd task1_ms
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
jupyter notebook
```

Linux / macOS:

```bash
git clone https://github.com/jruiz002/task1_ms.git
cd task1_ms
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

También se puede abrir la carpeta en VS Code y elegir el kernel de `.venv`.

Para re-ejecutar un notebook sin interfaz (regenera las figuras en `img/`), cambiando `Task2` por `Task1` o `Task3` según el caso:

```bash
jupyter nbconvert --to notebook --execute --inplace Task2.ipynb
```

## Autores

- José Gerardo Ruiz García – 23719
- Gerardo André Fernández Cruz – 23763
- Juan Diego Solís Martínez – 23720
