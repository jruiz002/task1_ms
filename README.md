# Hoja de Trabajo 6 – Competencia entre plataformas

Estudiamos un modelo de Lotka-Volterra competitivo entre dos plataformas con los parámetros del grupo 5. El Task 1 (análisis analítico) está en `Task1.ipynb`. El Task 2 (simulación numérica con Euler y RK4 propios, retrato de fases, cuencas de atracción, estabilidad local e intervenciones) está en `Task2.ipynb`.
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

Para re-ejecutar el notebook sin interfaz (regenera las figuras en `img/`):

```bash
jupyter nbconvert --to notebook --execute --inplace Task2.ipynb
```

## Autores

- José Gerardo Ruiz García – 23719
- Gerardo André Fernández Cruz – 23763
- Juan Diego Solís Martínez – 23720
