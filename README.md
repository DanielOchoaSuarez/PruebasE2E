# Proyecto Pruebas automatizadas

## Semana 5: Pruebas E2E

### Kraken

Escenarios:

- Como usuario de ghost creo un nuevo miembro
- Como usuario de ghost edito un miembro
- Como usuario de ghost elimino un miembro
- Como usuario de ghost creo un tag publico
- Como usuario de ghost edito un tag publico
- Como usuario de ghost elimino un tag publico
- Como usuario de ghost creo un tag interno
- Como usuario de ghost edito un tag interno
- Como usuario de ghost elimino un tag interno
- Como usuario de ghost configuro tema dark

### Versiones

La ejecución del test se realizó con las siguientes versiones:

- Windows 10 Pro
- npm 8.15.0
- node 16.17.1
- cucumber 7.2.1
- kraken-node 1.0.24
- Android Debug Bridge adb 1.0.41
- Ghost-CLI 1.23.1
- Ghost 5.18.0

### Ejecutar la prueba Kraken

Debido a la restricción de la herramienta Kraken en Windows, se debe seleccionar solo un archivo con un escenario en la carpeta features/ y asegurar que solo un archivo tenga la extensión .feature:

| Orden ejecución | Archivo            | Escenario                                    |
| --------------- | ------------------ | -------------------------------------------- |
| 1               | member_1.feature   | Como usuario de ghost creo un nuevo miembro  |
| 2               | member_2.feature   | Como usuario de ghost edito un miembro       |
| 3               | member_3.feature   | Como usuario de ghost elimino un miembro     |
| 4               | tag_1.feature      | Como usuario de ghost creo un tag publico    |
| 5               | tag_2.feature      | Como usuario de ghost edito un tag publico   |
| 6               | tag_3.feature      | Como usuario de ghost elimino un tag publico |
| 7               | tag_4.feature      | Como usuario de ghost creo un tag interno    |
| 8               | tag_5.feature      | Como usuario de ghost edito un tag interno   |
| 9               | tag_6.feature      | Como usuario de ghost elimino un tag interno |
| 10              | settings_1.feature | Como usuario de ghost configuro tema dark    |

Para ejecutar el test es necesario ubicarse en la misma ruta del archivo package.json del proyecto y ejecutar los siguientes comandos:

```
npm i
./node_modules/kraken-node/bin/kraken-node run
```