# Bioinformática en laboratorio — sesión 04

## Preparación

Clona el repositorio y ejecuta estos comandos desde su carpeta:

```bash
python -m pip install -r requirements.txt
jupyter lab
```

Abre `main.ipynb` y ejecuta las celdas en orden. La primera ejecución extrae
automáticamente la base de datos local incluida en `blastdb/`.

Para ejecutar el análisis BLAST local también necesitas **NCBI BLAST+**,
concretamente el programa `blastn`, instalado y disponible en el `PATH`.
BLAST+ es una herramienta externa y no se instala con `pip`. Si solo quieres
leer los resultados online incluidos en el repositorio, no necesitas BLAST+.

El cuaderno usa los XML de resultados online incluidos (`GN93KTEF016-Alignment.xml`
y `blastx_geiser.xml`), así que no hace falta volver a descargarlos.

## Archivos de la base de datos

`blastdb/16S_ribosomal_RNA.tar.gz` contiene la base de datos BLAST y los archivos
de taxonomía necesarios para el análisis local. Se conserva comprimida en Git
para reducir el tamaño del repositorio y se descomprime al ejecutar el cuaderno.