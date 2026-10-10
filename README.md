# NextCode Suite para Windows · versiones publicadas

Instaladores de **NextCode Suite para Windows**, el programa de gestión de [NextCode Agency](https://nextcodeagency.com):
facturación con VERI\*FACTU, clientes, presupuestos, cobros, contabilidad y el resto del panel, con los datos en tu
ordenador.

- **Descarga:** la última versión está en [Releases](../../releases/latest) y en
  [nextcodeagency.com/escritorio](https://nextcodeagency.com/escritorio).
- **Requisitos:** Windows 10 22H2 u 11 de 64 bits. Se instala por usuario, sin permisos de administrador.
- **Activación:** con la clave de licencia `NCS1-…` que te da NextCode.
- **Actualizaciones:** la propia app avisa de las versiones nuevas y se actualiza sola; si algo falla, vuelve a la
  versión anterior.

## Comprobar el instalador

Cada versión lleva `SHA256SUMS.txt` y el descriptor firmado `NextCodeSuite-<versión>.ncsr`. La app solo instala una
actualización si su firma, su tamaño y su suma SHA-256 coinciden. Para comprobar a mano el instalador descargado, en
PowerShell:

```powershell
Get-FileHash .\NextCodeSuite-Setup-<versión>.exe -Algorithm SHA256
```

El resultado tiene que ser el que aparece en `SHA256SUMS.txt` de esa versión.

## Aviso de Windows SmartScreen

Mientras el instalador no lleve firma de código, Windows puede mostrar «Windows protegió su PC». Para seguir, pulsa
**«Más información»** y después **«Ejecutar de todas formas»**.
