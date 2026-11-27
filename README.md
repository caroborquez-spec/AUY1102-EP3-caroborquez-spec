# AUY1102-EP3 — Pipeline CI/CD con GitHub Actions

Evaluación Parcial N° 3 — Ciclo de Vida del Software I.

Proyecto de ejemplo con una calculadora en Python, su suite de pruebas con pytest,
un sitio web de reservas publicado en GitHub Pages y un pipeline de CI/CD que
automatiza pruebas, análisis de seguridad (CodeQL) y despliegue.

## Pipeline

- **Pruebas unitarias**: `pytest -v` sobre `calculadora.py`.
- **Análisis CodeQL**: escaneo de seguridad con `security-extended`.
- **Despliegue en GitHub Pages**: publica `site/` solo si las dos etapas anteriores
  terminan en verde y el evento no es un pull request.

## Uso local

```bash
pip install -r requirements.txt
pip install pytest
pytest -v
```
