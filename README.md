# cord64

`cord64` es una librería de Python para convertir archivos a texto en Base64 y viceversa.

## Instalación

Para instalar la librería, solo pon en tu terminal:

```bash
pip install cord64
```
Uso
A continuación se muestra un ejemplo de cómo usar las funciones convert_archive_to_base64 y base64_to_archive:
```python
from cord64.convert import convert_archive_to_base64, base64_to_archive

# Ruta del archivo a convertir
file_path = "ruta/al/archivo/image.png"

# Carpeta donde se guardará el archivo decodificado
output_folder = "ruta/al/carpeta/output"

# Convertir archivo a Base64
base64_text = convert_archive_to_base64(file_path)
print(f"Archivo en Base64: {base64_text}")

# Convertir Base64 a archivo y guardarlo en la carpeta especificada
output_file_path = base64_to_archive(base64_text, output_folder, "image.png")
print(f"Archivo guardado en: {output_folder}")
```

## Funciones

convert_archive_to_base64(file_path)
Convierte un archivo a una cadena de texto en Base64.

- file_path: Ruta del archivo a convertir.

base64_to_archive(base64_text, folder_path, file_name)
Decodifica un texto en Base64 y guarda el archivo en la carpeta especificada.

- base64_text: Texto en Base64 a decodificar.
- folder_path: Carpeta donde se guardará el archivo decodificado.
- file_name: Nombre del archivo decodificado.

Licencia
Este proyecto está licenciado bajo la Licencia MIT